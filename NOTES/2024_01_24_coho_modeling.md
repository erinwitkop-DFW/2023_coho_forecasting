# January 24th, 2024

## GOALS

1. Create new Rstudio project
2. Load data
3. Run STAN model
4. Create running list of questions 

## NOTES

1. Create new RStudio project
    - Created new project
    - copied "stipm_2023.Rmd" to my new project
    - created working copy of the script and uploaded to github
    - Installed dependencies

2. Loading data 

    - First reviewing the data dependencies that go into the model 
    - Noting that I do not have the coho FRAM mdb and the fram coho escapement data that the model includes as a param
        # f_fram_mdb: "~/O/code/coho/fram_mdbs/PSC_CoTC_PostSeason_CohoFRAMDB_thru2021_021523.mdb"
#  f_fram_prelim_escp: "~/T/DFW-Salmon Mgmt Modeling Team - General/Escapement files/Coho/fram_coho_escapement_2023.xlsx"

3. Running code 

    - Column name questions: 
        - spwn, hvst, rtrn are all expanded values correct?

    - pop_id is the willapa bay naturals stockID 161

    - What does release scalar mean

    - Are there databases where I can lookup what some of these codes mean? like for example the tag_type code from RMIS

    - Ran into issue where I need admin approval to install Rtools! frustrating, means I can't run the STIPM and AR1 models just yet

    - Had to stop at running the one-ahead post-hoc performance evaluation

4. Questions:
    - Running data as prelim with smolts, CWTs escp and LM(LOG(HVST) ~ LOG(SPWN)) then you follow it up once the post-season MDB is available. This is the plan for this year correct? We start with the prelim data and rebuild from the post-season run database
    - We will be rebuilding fram from mdb correct?
    - I need the mdb files to be able to rebuild from the post-season run database
    - What is the release scalar mean in the RMIS hatchery survival release location document
    - Origin of all the supporting files, particularly the previous FRAM model runs that I don't have access to
    - Should we update the RMIS lookup data - that is the CWT releases and recoveries 
        - The release update file could be updated, currently only has data from 2010-2021 so we could add in 2022 data
        - The recoveries file was queried for recovery years 2019 onward - why not include previous years? I thought though that we were looking at age 3 fish? why are there so many brood year and recovery year combinations
        - They suggest repopulating these coho files "from scratch" with comprehensive query files. What does this mean - more years being queried?
        - What determines a questionable recovery year? Just having a large gap in brood year and recovery year and few fish? What is an adequate sample size here? 

    - Why are there different definitions for adult_pred and adult_est in the STIPM model vs the AR1 model? 

5. List of files to update for this upcoming year