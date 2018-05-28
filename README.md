# B2BO
B2BO Indicator 

## Creating Levels
The steps to creating the levels are as followed:
1. Draw Trigger Lines
2. Measure Max Distance of Each Oppurtunity/Window/Wave/Whatever you want to call it.
3. Draw the target bands using the mean cut off from the Frequency Distribution data in step 2.

### Drawing Trigger Lines
First we need to plot the 2 trigger lines that are drawn using MA Envelopes. In this example we are using the following inputs:
- Period: 50
- Deviations: 0.5

![alt text](https://github.com/ipbyrne/B2BO/blob/master/images/B2BO-triggers-only.PNG?raw=true "Trigger Lines Only")

### Gathering Distrance Data
Now that we have our trigger lines and slice the data into tradable windows. In the image below we can see the long oppurtunity start at the candle circled and labeled #1. This happens when a candle opens below the top band, and closes above it (vice versa for shorts). This long oppurtunity will be over when a candle touches the lower (high for shorts) band (this is important because it means when a long oppurtunity ends, a short one DOES NOT automatically open). The lines that end our oppurtunity (top line for shorts, bottom line for longs) acts as a constantly trailing Stop Loss.

![alt text](https://github.com/ipbyrne/B2BO/blob/master/images/B2BO-formation.PNG?raw=true "Example of Oppurtunities")

During each oppurtunity, we measure how high the price travels above (or below for shorts) are stop loss. This distance will be referred to as the spread. We then record the max distance.

### Drawing Target Bands
We then take our distance frequency data and find the 50% cut off distance, the 75% cut off distance, and the 87.5% cut off distance. This effectively forms there 3 levels, where when the level below is reached, it is 50/50 the spread will widen to the level above or go back to our SL.

We then get the pip value of these levels and draw the bands x amount of pips below/above our SL to form our targets.

![alt text](https://github.com/ipbyrne/B2BO/blob/master/images/B2BO-bands-added.PNG?raw=true "Price with MA Envelopes")

The orange line represents the 50% cut off. The blue line represents the 75% cut off, and the red line represents the 87.5% cut off.
Once a new oppurutnity forms, there is a 50/50 chance the spread will widen to reach the orange band.
Once the spread reaches the 50% cut off, it is now 50/50 it will widen to the blue line. If/when the spread widens to the blue line, it is now 50/50 it will widen to the red line.

## Current Issues/Complaints
Coming Soon...



