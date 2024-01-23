# January 22nd, 2024

## GOALS

1. Create new Github account for DFW
2. Clone repo 
3. Create new repo for my edits etc. 
4. Review notes from Dan Auerbach
5. Compile Questions for Dan 


## NOTES

1. Created new DFW github account

    - New account: https://github.com/erinwitkop-DFW

2. Cloned repo with coho ST-IPM

```PS C:\Users\wite1477\OneDrive - Washington State Executive Branch Agencies\Documents\FISH_MANAGEMENT\FORECASTING\COHO\2023> git clone https://github.com/wdfw-fp/coho_STIPM.git```

3. Push new folder with my notes to github

    - Added this path to a new github repository:PS C:\Users\wite1477\OneDrive - Washington State Executive Branch Agencies\Documents\FISH_MANAGEMENT\FORECASTING\COHO\2023\2023_RECREATE>

4. Review Notes:

    - 1/19/24: 
        From Dan Auerbach: "Hey Erin, I was chatting with Ty Garber this morning about a different coho product and asked about where things stand relative to the dataset updates from FRAM and RMIS. This note is to help me remember to try to explain next Friday what he’d pointed out about the RMIS lookup that he’d built awhile back and which gets used in the chunk starting L149 (wrangling the ‘rmis_recs_*’ and ‘rmis_releases_*’ files). You and I can look over that bit more closely (I didn’t have time today) and think about how critical it might be to update it. I can also explain where the supporting csv files come from, since I realized that’s not in this script.

        Along those lines, I think I said this on our call, but a good focus ahead of the 26th would be to not worry yet about the dataset updates, but just aim to get last years’ core dataset into memory (fram_cwt_smolt_fulljoin_for2023.csv) and see if you can get stan sampling on your machine, first running the two rstan::stan wrapper function chunks down in the “Model fitting” section and then the “full_data_fit” down on L946. There’s a bunch of lines related to assessing “one ahead” performance comparisons that we did for the SSC presentation and which could/should have future relevance (hence still being in there), but which we won’t need for now."

5. Compiled questions for next meeting

    1. Do we need to update code to pull data from RMIS?
    2. What data do we need to do for modeling hatchery coho?
