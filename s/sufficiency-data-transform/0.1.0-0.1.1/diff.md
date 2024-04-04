# Comparing `tmp/sufficiency_data_transform-0.1.0.tar.gz` & `tmp/sufficiency_data_transform-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sufficiency_data_transform-0.1.0.tar", max compression
+gzip compressed data, was "sufficiency_data_transform-0.1.1.tar", max compression
```

## Comparing `sufficiency_data_transform-0.1.0.tar` & `sufficiency_data_transform-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0      400 2024-04-04 11:56:51.444276 sufficiency_data_transform-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1035 2024-04-03 15:11:03.686177 sufficiency_data_transform-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-03 15:11:03.688176 sufficiency_data_transform-0.1.0/sufficiency_data_transform/__init__.py
--rw-r--r--   0        0        0      140 2024-04-03 15:11:03.689177 sufficiency_data_transform-0.1.0/sufficiency_data_transform/__main__.py
--rw-r--r--   0        0        0    18158 2024-04-04 08:36:23.094895 sufficiency_data_transform-0.1.0/sufficiency_data_transform/all_dim_and_fact.py
--rw-r--r--   0        0        0    21972 2024-04-03 15:11:03.693180 sufficiency_data_transform-0.1.0/sufficiency_data_transform/dim_maps.py
--rw-r--r--   0        0        0     3599 2024-04-03 15:11:03.694178 sufficiency_data_transform-0.1.0/sufficiency_data_transform/maps.py
--rw-r--r--   0        0        0     1248 2024-04-03 15:11:03.694178 sufficiency_data_transform-0.1.0/sufficiency_data_transform/utils.py
--rw-r--r--   0        0        0     1741 1970-01-01 00:00:00.000000 sufficiency_data_transform-0.1.0/setup.py
--rw-r--r--   0        0        0     1520 1970-01-01 00:00:00.000000 sufficiency_data_transform-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1022 2024-04-04 13:25:55.629162 sufficiency_data_transform-0.1.1/README.md
+-rw-r--r--   0        0        0      389 2024-04-04 13:25:55.629162 sufficiency_data_transform-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-04 13:25:55.629162 sufficiency_data_transform-0.1.1/sufficiency_data_transform/__init__.py
+-rw-r--r--   0        0        0      137 2024-04-04 13:25:55.629162 sufficiency_data_transform-0.1.1/sufficiency_data_transform/__main__.py
+-rw-r--r--   0        0        0    17858 2024-04-04 13:25:55.629162 sufficiency_data_transform-0.1.1/sufficiency_data_transform/all_dim_and_fact.py
+-rw-r--r--   0        0        0    21424 2024-04-04 13:25:55.629162 sufficiency_data_transform-0.1.1/sufficiency_data_transform/dim_maps.py
+-rw-r--r--   0        0        0     3484 2024-04-04 13:25:55.629162 sufficiency_data_transform-0.1.1/sufficiency_data_transform/maps.py
+-rw-r--r--   0        0        0     1202 2024-04-04 13:25:55.629162 sufficiency_data_transform-0.1.1/sufficiency_data_transform/utils.py
+-rw-r--r--   0        0        0     1570 1970-01-01 00:00:00.000000 sufficiency_data_transform-0.1.1/PKG-INFO
```

### Comparing `sufficiency_data_transform-0.1.0/README.md` & `sufficiency_data_transform-0.1.1/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-This is a temporary repo that hosts code which needs to be plugged into the liia-tools-pipeline.
-
-The input data used in this process are the output files generated at the end of the 903 pipeline.
-
-## Setup
-1. Create a `.env` file whose content should be a copy of the `env.sample` file.
-2. In your `.env` file, assign the input and output variables to directories you choose. Ensure that your path ends with `\`.
-3. In the command line, do `poetry install` and then `poetry shell` to install dependencies.
-4. Then `python -m sufficiency_data_transform` to run the tool and generate the output files.
-
-Dummy input data can be gotten from [this location](https://socialfinanceltd.sharepoint.com/:f:/s/Digi/Elr6MmNuznVBm6M3YWSlXqIBWRTv6Pb19eVe2HI_FdTXjw?e=TbZQYL). Care should be taken so that it is **never pushed** on GitHub. 
-You can create an empty directory to which the outputs should be sent.
-
+This is a temporary repo that hosts code which needs to be plugged into the liia-tools-pipeline.
+
+The input data used in this process are the output files generated at the end of the 903 pipeline.
+
+## Setup
+1. Create a `.env` file whose content should be a copy of the `env.sample` file.
+2. In your `.env` file, assign the input and output variables to directories you choose. Ensure that your path ends with `\`.
+3. In the command line, do `poetry install` and then `poetry shell` to install dependencies.
+4. Then `python -m sufficiency_data_transform` to run the tool and generate the output files.
+
+Dummy input data can be gotten from [this location](https://socialfinanceltd.sharepoint.com/:f:/s/Digi/Elr6MmNuznVBm6M3YWSlXqIBWRTv6Pb19eVe2HI_FdTXjw?e=TbZQYL). Care should be taken so that it is **never pushed** on GitHub. 
+You can create an empty directory to which the outputs should be sent.
+
 In production, the goal will be to return the new output files to the same location where the input files were gotten from.
```

### Comparing `sufficiency_data_transform-0.1.0/sufficiency_data_transform/all_dim_and_fact.py` & `sufficiency_data_transform-0.1.1/sufficiency_data_transform/all_dim_and_fact.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,301 +1,301 @@
-import pandas as pd
-from decouple import config
-from sufficiency_data_transform.dim_maps import category_of_need, legal_status, ofsted_effectiveness, placement_provider, placement_type, reason_episode_ceased, reason_for_new_episode, reason_place_change
-from sufficiency_data_transform.maps import ons_map, dimLookedAfterChild_columns_map, gender_map, ethnic_description_map, uasc_status_map, ofsted_provider_map, ofsted_to_ons_map, postcodes_map, episodes_map, inspection_map
-from sufficiency_data_transform.utils import generate_dim, add_nan_row, fillna_date_columns, fillna_categorical_columns, check_encoding
-
-output_location = config('OUTPUT_LOCATION')
-input_location_ext = config('INPUT_LOCATION_EXT')
-input_location_903 = config('INPUT_LOCATION_903')
-
-def create_dim_tables():
-    """Create lookup tables"""
-    generate_dim(category_of_need, f'{output_location}dimCategoryOfNeed.csv')
-    generate_dim(legal_status, f'{output_location}dimLegalStatus.csv')
-    generate_dim(ofsted_effectiveness, f'{output_location}dimOfstedEffectiveness.csv')
-    generate_dim(placement_provider, f'{output_location}dimPlacementProvider.csv')
-    generate_dim(placement_type, f'{output_location}dimPlacementType.csv')
-    generate_dim(reason_episode_ceased, f'{output_location}dimReasonEpisodeCeased.csv')
-    generate_dim(reason_for_new_episode, f'{output_location}dimReasonForNewEpisode.csv')
-    generate_dim(reason_place_change, f'{output_location}dimReasonPlaceChange.csv')   
-
-def create_dimONSArea():
-    ons_area = pd.read_csv(f"{input_location_ext}ONS Area\ONS Area.csv")
-    ons_area.rename(columns=ons_map, inplace=True)
-
-    ons_area.drop(columns=["OBJECTID"], inplace=True)
-    # area code should be unknown only if all the possible codes are unknown
-    ward_df = ons_area
-    ward_df["AreaType"] = "Ward"
-    ward_df["AreaCode"] = ward_df["WardCode"]
-    ward_df["AreaName"] = ward_df["WardName"]
-
-    la_df = ons_area[['LACode', 'LAName', 'CountyCode', 'CountyName', 'RegionCode', 'RegionName', 'CountryCode', 'CountryName']]
-    la_df["AreaType"] = "LA"
-    la_df.loc[~la_df["LACode"].isna(), "AreaCode"] = la_df["LACode"]
-    la_df.loc[~la_df["LAName"].isna(), "AreaName"] = la_df["LAName"]
-
-    county_df = ons_area[['CountyCode', 'CountyName', 'RegionCode', 'RegionName', 'CountryCode', 'CountryName']]
-    county_df["AreaType"] = "County" 
-    county_df.loc[~county_df["CountyCode"].isna(), "AreaCode"] = county_df["CountyCode"]
-    county_df.loc[~county_df["CountyName"].isna(), "AreaName"] = county_df["CountyName"]
-
-    region_df = ons_area[['RegionCode', 'RegionName', 'CountryCode', 'CountryName']]
-    region_df["AreaType"] = "Region" 
-    region_df.loc[~region_df["RegionCode"].isna(), "AreaCode"] = region_df["RegionCode"]
-    region_df.loc[~region_df["RegionName"].isna(), "AreaName"] = region_df["RegionName"]
-
-    country_df = ons_area[['CountryCode', 'CountryName']]
-    country_df["AreaType"] = "Country"
-    country_df.loc[~country_df["CountryCode"].isna(), "AreaCode"] = country_df["CountryCode"]
-    country_df.loc[~country_df["CountryName"].isna(), "AreaName"] = country_df["CountryName"]
-
-    dimONSArea = pd.concat([ward_df, la_df, county_df, region_df, country_df]).drop_duplicates()
-
-    dimONSArea.reset_index(drop=True)
-    dimONSArea.reset_index(inplace=True, names="ONSAreaKey")
-
-    # add a row that simulates the scenario where all values are nan
-    dimONSArea = add_nan_row(dimONSArea, "ONSAreaKey")
-    dimONSArea.to_csv(f"{output_location}dimONSArea.csv", index=False)
-
-def create_dimLookedAfterChild():
-    header = pd.read_csv(f"{input_location_903}pan_London_SSDA903_Header.csv")
-    uasc = pd.read_csv(f"{input_location_903}pan_London_SSDA903_UASC.csv")
-    
-    ons_area = pd.read_csv(f"{output_location}dimONSArea.csv")
-    ons_area = ons_area[["ONSAreaKey", "AreaName"]]
-
-    dimLookedAfterChild = header.merge(uasc, on=['CHILD', "SEX", "DOB", "LA", "YEAR"], how='left')
-
-    dimLookedAfterChild.rename(columns=dimLookedAfterChild_columns_map, inplace=True)
-    dimLookedAfterChild["Gender"] = dimLookedAfterChild["Gender"].map(gender_map).fillna("Not Specified")
-    dimLookedAfterChild["EthnicDescription"] = dimLookedAfterChild.EthnicCode.map(ethnic_description_map)
-
-    dimLookedAfterChild["UASCStatusCode"] = dimLookedAfterChild.UASCCeasedDateKey.map(lambda x: 0 if pd.isnull(x) else 1) 
-    dimLookedAfterChild["UASCStatusDescription"] = dimLookedAfterChild.UASCStatusCode.map(uasc_status_map) 
-
-    dimLookedAfterChild = dimLookedAfterChild.merge(ons_area, left_on="LA", right_on="AreaName", how="left")
-    dimLookedAfterChild.rename(columns={"ONSAreaKey": "ONSAreaCode"}, inplace=True)
-    # remove name columns since they are not present in output
-    dimLookedAfterChild.drop(columns=["AreaName", "LA"], inplace=True)
-
-    date_cols = ["DateOfBirthKey", "UASCCeasedDateKey"] # these are used to generate other columns above so should only be changed here at the end.
-    dimLookedAfterChild = fillna_date_columns(dimLookedAfterChild, date_cols)    
-
-    dimLookedAfterChild["Gender"] = dimLookedAfterChild["Gender"].fillna("Not Specified")
-    dimLookedAfterChild["EthnicCode"] = dimLookedAfterChild["EthnicCode"].fillna("UNKNOWN")
-    dimLookedAfterChild["ChildIdentifier"] = dimLookedAfterChild["ChildIdentifier"].fillna("UNKNOWN CHILD")
-
-    categorical_cols = ["SubmissionYearDateKey", "EthnicDescription", "UASCStatusCode", "UASCStatusDescription", "ONSAreaCode"] # replace nans in ons area code
-    dimLookedAfterChild = fillna_categorical_columns(dimLookedAfterChild, categorical_cols)
-
-    dimLookedAfterChild.reset_index(inplace=True, drop=True)
-    dimLookedAfterChild.reset_index(inplace=True, names="LookedAfterChildKey")
-
-    dimLookedAfterChild.to_csv(f"{output_location}dimLookedAfterChild.csv", index=False)
-
-def create_dimOfstedProvider():
-    providers_places_31Aug = pd.read_csv(f"{input_location_ext}Ofsted data\Providers+places_at_31_Aug_2023.csv")
-    closed_children_homes = pd.read_csv(f'{input_location_ext}Ofsted data\Closed_childrens_homes_31Mar23.csv')
-
-    ons_area = pd.read_csv(f"{output_location}dimONSArea.csv")
-    ons_area = ons_area[["ONSAreaKey", "AreaName"]]
-
-    dimOfstedProvider = providers_places_31Aug.merge(closed_children_homes, on=["URN", "Registration status"], how='outer')
-    dimOfstedProvider = dimOfstedProvider.drop_duplicates(subset="URN", keep="last")
-
-    dimOfstedProvider = dimOfstedProvider.rename(columns=ofsted_provider_map)
-    dimOfstedProvider = dimOfstedProvider[['URN', 'ProviderType', "Sector", 'RegistrationDate', 'ProviderStatus', 'ClosedDate', 'MaxUsers', 'OwnerName', "Local authority"]]
-
-    # these come in the data and do not have to be created
-    unknown_markers = ["NOTREC", "XXXXXXX", "UNKNOWN"]
-    dimOfstedProvider.loc[dimOfstedProvider["URN"].isin(unknown_markers), "UnknownSourceFlag"] = "TRUE"
-    dimOfstedProvider["UnknownSourceFlag"].fillna("FALSE", inplace=True)
-    dimOfstedProvider[dimOfstedProvider["UnknownSourceFlag"] == "TRUE"]
-
-    dimOfstedProvider["Local Authority"] = dimOfstedProvider["Local authority"].replace(ofsted_to_ons_map)
-
-    dimOfstedProvider = dimOfstedProvider.merge(ons_area, left_on="Local Authority", right_on="AreaName", how="left")
-    dimOfstedProvider = dimOfstedProvider.drop(columns=["Local Authority", "AreaName"])
-    dimOfstedProvider = dimOfstedProvider.rename(columns={"ONSAreaKey":"ONSAreaCode"})
-    
-    # Create OfstedProviderKey
-    dimOfstedProvider.reset_index(drop=True, inplace=True)
-    dimOfstedProvider.reset_index(inplace=True, names="OfstedProviderKey")
-    # ["URN"] == "UNKNOWN" etc can only exist in the fact table, not the dimension table.
-
-    # return key -3 if fact table sends a nan
-    nan_col = {col:pd.NA for col in dimOfstedProvider.columns}
-    nan_col["OfstedProviderKey"] = -3
-    dimOfstedProvider.loc[len(dimOfstedProvider)] = nan_col
-
-    # URNs that found no match in this table will return nans be given key -1 in the source table.
-
-    # return key -2 when incoming URN is XXXXXXX in docs.
-    nan_col = {col:pd.NA for col in dimOfstedProvider.columns}
-    nan_col["URN"] = "XXXXXXX"
-    nan_col["OfstedProviderKey"] = -2
-    dimOfstedProvider.loc[len(dimOfstedProvider)] = nan_col
-
-    # replace nans
-    categorical_columns = ["ProviderType", "Sector", "ProviderStatus", "MaxUsers", "OwnerName", "Local authority", "UnknownSourceFlag"]
-    date_columns = ["RegistrationDate", "ClosedDate"]
-    dimOfstedProvider = fillna_categorical_columns(dimOfstedProvider, categorical_columns)
-    dimOfstedProvider = fillna_date_columns(dimOfstedProvider, date_columns)
-
-    # select relevant columns
-    dimOfstedProvider = dimOfstedProvider[['OfstedProviderKey', 'URN', 'ProviderType', 'Sector', 'RegistrationDate', 'ProviderStatus', 'ClosedDate', 'MaxUsers', 'UnknownSourceFlag', 'ONSAreaCode', 'OwnerName', ]]
-
-    dimOfstedProvider.to_csv(f"{output_location}dimOfstedProvider.csv", index=False)
-
-def create_dimPostcode():
-    postcodes = pd.read_csv(f"{input_location_ext}Postcode directory\ONSPD reduced to postcode sector.csv")
-    postcodes = postcodes[["pcd2", "lat", "long", "oseast1m", "osnrth1m", "imd", "oslaua", "lsoa11"]]
-
-    dimPostcode = postcodes.rename(postcodes_map, axis=1)
-
-    dimPostcode.reset_index(inplace=True, drop=True)
-    dimPostcode.reset_index(inplace=True, names="PostcodeKey")
-    dimPostcode = add_nan_row(dimPostcode, "PostcodeKey")
-
-    dimPostcode = fillna_categorical_columns(dimPostcode, list(dimPostcode.columns))
-    dimPostcode.to_csv(f"{output_location}dimPostcode.csv", index=False)
-
-def create_factEpisode():
-    episodes = pd.read_csv(f'{input_location_903}pan_London_SSDA903_Episodes.csv')
-
-    looked_after_child = pd.read_csv(f"{output_location}dimLookedAfterChild.csv")
-    reason_for_new_episode = pd.read_csv(f"{output_location}dimReasonForNewEpisode.csv")
-    legal_status = pd.read_csv(f"{output_location}dimLegalStatus.csv")
-    category_of_need = pd.read_csv(f"{output_location}dimCategoryOfNeed.csv")
-    placement_type = pd.read_csv(f"{output_location}dimPlacementType.csv")
-    placement_provider = pd.read_csv(f"{output_location}dimPlacementProvider.csv")
-    reason_episode_ceased = pd.read_csv(f"{output_location}dimReasonEpisodeCeased.csv")
-    reason_place_change = pd.read_csv(f"{output_location}dimReasonPlaceChange.csv")
-    postcode = pd.read_csv(f"{output_location}dimPostcode.csv")
-    ofsted_provider = pd.read_csv(f"{output_location}dimOfstedProvider.csv")
-    ons_area = pd.read_csv(f"{output_location}dimONSArea.csv")
-
-    # LookedAfterChildKey
-    episodes = episodes.merge(looked_after_child, left_on='CHILD', right_on='ChildIdentifier', how='left')
-
-    # ReasonForNewEpisodeKey
-    episodes = episodes.merge(reason_for_new_episode, left_on='RNE', right_on='ReasonForNewEpisodeCode', how='left')
-
-    # LegalStatusKey
-    episodes = episodes.merge(legal_status, left_on='LS', right_on='LegalStatusCode', how='left')
-
-    # CategoryOfNeedKey
-    episodes = episodes.merge(category_of_need, left_on='CIN', right_on='CategoryOfNeedCode', how='left')
-
-    # PlacementTypeKey
-    episodes = episodes.merge(placement_type, left_on='PLACE', right_on='PlacementTypeCode', how='left')
-
-    # PlacementProviderKey
-    episodes = episodes.merge(placement_provider, left_on='PLACE_PROVIDER', right_on='PlacementProviderCode', how='left')
-
-    # ReasonEpisodeCeasedKey
-    episodes = episodes.merge(reason_episode_ceased, left_on='REC', right_on='ReasonEpisodeCeasedCode', how='left')
-
-    # ReasonPlaceChangeKey
-    episodes = episodes.merge(reason_place_change, left_on='REASON_PLACE_CHANGE', right_on='ReasonPlaceChangeCode', how='left')
-
-    # OfstedProviderKey
-    ofsted_provider.URN = ofsted_provider.URN.astype(str)
-    episodes.URN = episodes.URN.astype(str)
-    episodes = episodes.merge(ofsted_provider, left_on='URN', right_on='URN', how='left')
-
-    # ONSAreaKey
-    episodes = episodes.merge(ons_area, left_on='LA', right_on='AreaName', how='left')
-
-    postcode = postcode[["PostcodeKey", "Sector"]]
-    # HomePostcodeKey
-    episodes = episodes.merge(postcode, left_on='HOME_POST', right_on='Sector', how='left')
-    episodes = episodes.rename(columns={"PostcodeKey": "HomePostcodeKey"})
-
-    # PlacementPostcodeKey
-    episodes = episodes.merge(postcode, left_on='PL_POST', right_on='Sector', how='left')
-    episodes = episodes.rename(columns={"PostcodeKey": "PlacementPostcodeKey"})
-
-    episodes.rename(columns=episodes_map, inplace=True)
-    episodes = episodes[["LookedAfterChildKey", "EpisodeCommencedDateKey", "ReasonForNewEpisodeKey", "LegalStatusKey", "CategoryOfNeedKey", "PlacementTypeKey", "PlacementProviderKey", "EpisodeCeasedDateKey",  "ReasonEpisodeCeasedKey", "ReasonPlaceChangeKey", "HomePostcodeKey", "PlacementPostcodeKey", "OfstedProviderKey", "ONSAreaKey", "SubmissionYearDateKey"]]
-
-    # any missing keys after merge should be replaced with -1
-    episode_key_columns = ["LookedAfterChildKey", "EpisodeCommencedDateKey", "ReasonForNewEpisodeKey", "LegalStatusKey", "CategoryOfNeedKey", "PlacementTypeKey", "PlacementProviderKey", "EpisodeCeasedDateKey",  "ReasonEpisodeCeasedKey", "ReasonPlaceChangeKey", "HomePostcodeKey", "PlacementPostcodeKey", "OfstedProviderKey", "ONSAreaKey", "SubmissionYearDateKey"]
-    episodes = fillna_categorical_columns(episodes, episode_key_columns)
-    
-    episodes.to_csv(f"{output_location}Output data\\factEpisode.csv", index=False)
-
-def create_factOfstedInspection():
-    ofsted_effectiveness = pd.read_csv(f'{output_location}dimOfstedEffectiveness.csv')
-    ofsted_provider = pd.read_csv(f'{output_location}dimOfstedProvider.csv')
-
-    provider_level_at_31Aug = pd.read_csv(f'{input_location_ext}Ofsted data\Provider_level_at_31_Aug_2023.csv')
-
-    # This sample file returned a UnicodeDecodeError so it was necessary to check that it is read with the right encoding type. 
-    # leaving in the safeguard until it works in production with the real file.
-    encoding = check_encoding(f'{input_location_ext}Ofsted data/Provider_level_in_year_2022-23.csv')
-    provider_level_in_year_2022_23 = pd.read_csv(f"{input_location_ext}Ofsted data/Provider_level_in_year_2022-23.csv", encoding=encoding)
-
-    # provider_level_in_year_2022_23 was observed to contain several unnamed empty columns.
-    unnamed_columns = [col for col in provider_level_in_year_2022_23.columns if 'Unnamed' in col]
-    provider_level_in_year_2022_23 = provider_level_in_year_2022_23.drop(columns=unnamed_columns)
-
-    # rename inspection date column in provider_level_at_31Aug so that they match when concatenated.
-    provider_level_at_31Aug = provider_level_at_31Aug.rename(columns={'Latest full inspection date': 'Inspection date',})
-    
-    factOfstedInspection = pd.concat([provider_level_in_year_2022_23, provider_level_at_31Aug])
-    factOfstedInspection = factOfstedInspection.drop_duplicates(subset=['URN', 'Inspection date'], keep='first')
-
-    # create IsLatest column that indicates if inspection is the most recent one recorded for a URN
-    factOfstedInspection["IsLatest"] = factOfstedInspection.groupby('URN')['Inspection date'].transform('max') == factOfstedInspection['Inspection date']
-
-    # Update the EndDate where isLatest is True with 2999 if EndDate is missing, otherwise keep it the same as InspectionDateKey
-    factOfstedInspection.loc[factOfstedInspection['IsLatest'] == True, 'EndDateKey'] = factOfstedInspection.loc[factOfstedInspection['IsLatest'] == True, 'Inspection date']
-    factOfstedInspection['EndDateKey'].fillna('2999-12-31', inplace=True)
-
-    # Find the next inspection date for each row where isLatest is False
-    next_inspection_dates = factOfstedInspection.loc[factOfstedInspection['IsLatest'] == False, 'Inspection date'].shift(-1)
-
-    # Update the EndDate where isLatest is False with the next inspection date
-    factOfstedInspection.loc[factOfstedInspection['IsLatest'] == False, 'EndDateKey'] = next_inspection_dates
-
-    factOfstedInspection = factOfstedInspection.rename(columns=inspection_map)
-    factOfstedInspection = factOfstedInspection[["InspectionDateKey", "EndDateKey", "OwnerName", "Effectiveness", "IsLatest"]]
-
-    factOfstedInspection.IsLatest = factOfstedInspection.IsLatest.map({True: "TRUE", False: "FALSE"})
-
-    # fill nans
-    categorical_columns = ["OwnerName"]
-    factOfstedInspection = fillna_categorical_columns(factOfstedInspection, categorical_columns)
-    date_columns = ["InspectionDateKey", "EndDateKey"]
-    factOfstedInspection = fillna_date_columns(factOfstedInspection, date_columns)
-    
-    # create OfstedEffectivenessKey
-    factOfstedInspection['Effectiveness'] = factOfstedInspection['Effectiveness'].fillna('Unknown')
-    factOfstedInspection = factOfstedInspection.merge(ofsted_effectiveness, how='left', left_on='Effectiveness', right_on='OverallEffectiveness')
-    factOfstedInspection = factOfstedInspection.drop(columns=['Effectiveness', 'OverallEffectiveness', 'Grade'])
-
-    # create OfstedProviderKey
-    ofsted_provider = ofsted_provider[['OfstedProviderKey', 'OwnerName']]
-    factOfstedInspection = factOfstedInspection.merge(ofsted_provider, how='left', on='OwnerName')
-    factOfstedInspection = factOfstedInspection.drop(columns=['OwnerName'])
-
-    # replace keys that couldn't be matched with -1
-    key_columns = ['OfstedProviderKey', 'OfstedEffectivenessKey']
-    factOfstedInspection = fillna_categorical_columns(factOfstedInspection, key_columns)
-
-    factOfstedInspection.reset_index(inplace=True, drop=True)
-    factOfstedInspection.reset_index(inplace=True, names='factOfstedInspectionKey')
-
-    factOfstedInspection.to_csv(f'{output_location}factOfstedInspection.csv', index=False)
-
-def create_sufficiency_data():
-    create_dim_tables()
-    create_dimONSArea()
-    create_dimLookedAfterChild()
-    create_dimOfstedProvider()
-    create_dimPostcode()
-    create_factEpisode()
+import pandas as pd
+from decouple import config
+from sufficiency_data_transform.dim_maps import category_of_need, legal_status, ofsted_effectiveness, placement_provider, placement_type, reason_episode_ceased, reason_for_new_episode, reason_place_change
+from sufficiency_data_transform.maps import ons_map, dimLookedAfterChild_columns_map, gender_map, ethnic_description_map, uasc_status_map, ofsted_provider_map, ofsted_to_ons_map, postcodes_map, episodes_map, inspection_map
+from sufficiency_data_transform.utils import generate_dim, add_nan_row, fillna_date_columns, fillna_categorical_columns, check_encoding
+
+output_location = config('OUTPUT_LOCATION')
+input_location_ext = config('INPUT_LOCATION_EXT')
+input_location_903 = config('INPUT_LOCATION_903')
+
+def create_dim_tables():
+    """Create lookup tables"""
+    generate_dim(category_of_need, f'{output_location}dimCategoryOfNeed.csv')
+    generate_dim(legal_status, f'{output_location}dimLegalStatus.csv')
+    generate_dim(ofsted_effectiveness, f'{output_location}dimOfstedEffectiveness.csv')
+    generate_dim(placement_provider, f'{output_location}dimPlacementProvider.csv')
+    generate_dim(placement_type, f'{output_location}dimPlacementType.csv')
+    generate_dim(reason_episode_ceased, f'{output_location}dimReasonEpisodeCeased.csv')
+    generate_dim(reason_for_new_episode, f'{output_location}dimReasonForNewEpisode.csv')
+    generate_dim(reason_place_change, f'{output_location}dimReasonPlaceChange.csv')   
+
+def create_dimONSArea():
+    ons_area = pd.read_csv(f"{input_location_ext}ONS Area\ONS Area.csv")
+    ons_area.rename(columns=ons_map, inplace=True)
+
+    ons_area.drop(columns=["OBJECTID"], inplace=True)
+    # area code should be unknown only if all the possible codes are unknown
+    ward_df = ons_area
+    ward_df["AreaType"] = "Ward"
+    ward_df["AreaCode"] = ward_df["WardCode"]
+    ward_df["AreaName"] = ward_df["WardName"]
+
+    la_df = ons_area[['LACode', 'LAName', 'CountyCode', 'CountyName', 'RegionCode', 'RegionName', 'CountryCode', 'CountryName']]
+    la_df["AreaType"] = "LA"
+    la_df.loc[~la_df["LACode"].isna(), "AreaCode"] = la_df["LACode"]
+    la_df.loc[~la_df["LAName"].isna(), "AreaName"] = la_df["LAName"]
+
+    county_df = ons_area[['CountyCode', 'CountyName', 'RegionCode', 'RegionName', 'CountryCode', 'CountryName']]
+    county_df["AreaType"] = "County" 
+    county_df.loc[~county_df["CountyCode"].isna(), "AreaCode"] = county_df["CountyCode"]
+    county_df.loc[~county_df["CountyName"].isna(), "AreaName"] = county_df["CountyName"]
+
+    region_df = ons_area[['RegionCode', 'RegionName', 'CountryCode', 'CountryName']]
+    region_df["AreaType"] = "Region" 
+    region_df.loc[~region_df["RegionCode"].isna(), "AreaCode"] = region_df["RegionCode"]
+    region_df.loc[~region_df["RegionName"].isna(), "AreaName"] = region_df["RegionName"]
+
+    country_df = ons_area[['CountryCode', 'CountryName']]
+    country_df["AreaType"] = "Country"
+    country_df.loc[~country_df["CountryCode"].isna(), "AreaCode"] = country_df["CountryCode"]
+    country_df.loc[~country_df["CountryName"].isna(), "AreaName"] = country_df["CountryName"]
+
+    dimONSArea = pd.concat([ward_df, la_df, county_df, region_df, country_df]).drop_duplicates()
+
+    dimONSArea.reset_index(drop=True)
+    dimONSArea.reset_index(inplace=True, names="ONSAreaKey")
+
+    # add a row that simulates the scenario where all values are nan
+    dimONSArea = add_nan_row(dimONSArea, "ONSAreaKey")
+    dimONSArea.to_csv(f"{output_location}dimONSArea.csv", index=False)
+
+def create_dimLookedAfterChild():
+    header = pd.read_csv(f"{input_location_903}pan_London_SSDA903_Header.csv")
+    uasc = pd.read_csv(f"{input_location_903}pan_London_SSDA903_UASC.csv")
+    
+    ons_area = pd.read_csv(f"{output_location}dimONSArea.csv")
+    ons_area = ons_area[["ONSAreaKey", "AreaName"]]
+
+    dimLookedAfterChild = header.merge(uasc, on=['CHILD', "SEX", "DOB", "LA", "YEAR"], how='left')
+
+    dimLookedAfterChild.rename(columns=dimLookedAfterChild_columns_map, inplace=True)
+    dimLookedAfterChild["Gender"] = dimLookedAfterChild["Gender"].map(gender_map).fillna("Not Specified")
+    dimLookedAfterChild["EthnicDescription"] = dimLookedAfterChild.EthnicCode.map(ethnic_description_map)
+
+    dimLookedAfterChild["UASCStatusCode"] = dimLookedAfterChild.UASCCeasedDateKey.map(lambda x: 0 if pd.isnull(x) else 1) 
+    dimLookedAfterChild["UASCStatusDescription"] = dimLookedAfterChild.UASCStatusCode.map(uasc_status_map) 
+
+    dimLookedAfterChild = dimLookedAfterChild.merge(ons_area, left_on="LA", right_on="AreaName", how="left")
+    dimLookedAfterChild.rename(columns={"ONSAreaKey": "ONSAreaCode"}, inplace=True)
+    # remove name columns since they are not present in output
+    dimLookedAfterChild.drop(columns=["AreaName", "LA"], inplace=True)
+
+    date_cols = ["DateOfBirthKey", "UASCCeasedDateKey"] # these are used to generate other columns above so should only be changed here at the end.
+    dimLookedAfterChild = fillna_date_columns(dimLookedAfterChild, date_cols)    
+
+    dimLookedAfterChild["Gender"] = dimLookedAfterChild["Gender"].fillna("Not Specified")
+    dimLookedAfterChild["EthnicCode"] = dimLookedAfterChild["EthnicCode"].fillna("UNKNOWN")
+    dimLookedAfterChild["ChildIdentifier"] = dimLookedAfterChild["ChildIdentifier"].fillna("UNKNOWN CHILD")
+
+    categorical_cols = ["SubmissionYearDateKey", "EthnicDescription", "UASCStatusCode", "UASCStatusDescription", "ONSAreaCode"] # replace nans in ons area code
+    dimLookedAfterChild = fillna_categorical_columns(dimLookedAfterChild, categorical_cols)
+
+    dimLookedAfterChild.reset_index(inplace=True, drop=True)
+    dimLookedAfterChild.reset_index(inplace=True, names="LookedAfterChildKey")
+
+    dimLookedAfterChild.to_csv(f"{output_location}dimLookedAfterChild.csv", index=False)
+
+def create_dimOfstedProvider():
+    providers_places_31Aug = pd.read_csv(f"{input_location_ext}Ofsted data\Providers+places_at_31_Aug_2023.csv")
+    closed_children_homes = pd.read_csv(f'{input_location_ext}Ofsted data\Closed_childrens_homes_31Mar23.csv')
+
+    ons_area = pd.read_csv(f"{output_location}dimONSArea.csv")
+    ons_area = ons_area[["ONSAreaKey", "AreaName"]]
+
+    dimOfstedProvider = providers_places_31Aug.merge(closed_children_homes, on=["URN", "Registration status"], how='outer')
+    dimOfstedProvider = dimOfstedProvider.drop_duplicates(subset="URN", keep="last")
+
+    dimOfstedProvider = dimOfstedProvider.rename(columns=ofsted_provider_map)
+    dimOfstedProvider = dimOfstedProvider[['URN', 'ProviderType', "Sector", 'RegistrationDate', 'ProviderStatus', 'ClosedDate', 'MaxUsers', 'OwnerName', "Local authority"]]
+
+    # these come in the data and do not have to be created
+    unknown_markers = ["NOTREC", "XXXXXXX", "UNKNOWN"]
+    dimOfstedProvider.loc[dimOfstedProvider["URN"].isin(unknown_markers), "UnknownSourceFlag"] = "TRUE"
+    dimOfstedProvider["UnknownSourceFlag"].fillna("FALSE", inplace=True)
+    dimOfstedProvider[dimOfstedProvider["UnknownSourceFlag"] == "TRUE"]
+
+    dimOfstedProvider["Local Authority"] = dimOfstedProvider["Local authority"].replace(ofsted_to_ons_map)
+
+    dimOfstedProvider = dimOfstedProvider.merge(ons_area, left_on="Local Authority", right_on="AreaName", how="left")
+    dimOfstedProvider = dimOfstedProvider.drop(columns=["Local Authority", "AreaName"])
+    dimOfstedProvider = dimOfstedProvider.rename(columns={"ONSAreaKey":"ONSAreaCode"})
+    
+    # Create OfstedProviderKey
+    dimOfstedProvider.reset_index(drop=True, inplace=True)
+    dimOfstedProvider.reset_index(inplace=True, names="OfstedProviderKey")
+    # ["URN"] == "UNKNOWN" etc can only exist in the fact table, not the dimension table.
+
+    # return key -3 if fact table sends a nan
+    nan_col = {col:pd.NA for col in dimOfstedProvider.columns}
+    nan_col["OfstedProviderKey"] = -3
+    dimOfstedProvider.loc[len(dimOfstedProvider)] = nan_col
+
+    # URNs that found no match in this table will return nans be given key -1 in the source table.
+
+    # return key -2 when incoming URN is XXXXXXX in docs.
+    nan_col = {col:pd.NA for col in dimOfstedProvider.columns}
+    nan_col["URN"] = "XXXXXXX"
+    nan_col["OfstedProviderKey"] = -2
+    dimOfstedProvider.loc[len(dimOfstedProvider)] = nan_col
+
+    # replace nans
+    categorical_columns = ["ProviderType", "Sector", "ProviderStatus", "MaxUsers", "OwnerName", "Local authority", "UnknownSourceFlag"]
+    date_columns = ["RegistrationDate", "ClosedDate"]
+    dimOfstedProvider = fillna_categorical_columns(dimOfstedProvider, categorical_columns)
+    dimOfstedProvider = fillna_date_columns(dimOfstedProvider, date_columns)
+
+    # select relevant columns
+    dimOfstedProvider = dimOfstedProvider[['OfstedProviderKey', 'URN', 'ProviderType', 'Sector', 'RegistrationDate', 'ProviderStatus', 'ClosedDate', 'MaxUsers', 'UnknownSourceFlag', 'ONSAreaCode', 'OwnerName', ]]
+
+    dimOfstedProvider.to_csv(f"{output_location}dimOfstedProvider.csv", index=False)
+
+def create_dimPostcode():
+    postcodes = pd.read_csv(f"{input_location_ext}Postcode directory\ONSPD reduced to postcode sector.csv")
+    postcodes = postcodes[["pcd2", "lat", "long", "oseast1m", "osnrth1m", "imd", "oslaua", "lsoa11"]]
+
+    dimPostcode = postcodes.rename(postcodes_map, axis=1)
+
+    dimPostcode.reset_index(inplace=True, drop=True)
+    dimPostcode.reset_index(inplace=True, names="PostcodeKey")
+    dimPostcode = add_nan_row(dimPostcode, "PostcodeKey")
+
+    dimPostcode = fillna_categorical_columns(dimPostcode, list(dimPostcode.columns))
+    dimPostcode.to_csv(f"{output_location}dimPostcode.csv", index=False)
+
+def create_factEpisode():
+    episodes = pd.read_csv(f'{input_location_903}pan_London_SSDA903_Episodes.csv')
+
+    looked_after_child = pd.read_csv(f"{output_location}dimLookedAfterChild.csv")
+    reason_for_new_episode = pd.read_csv(f"{output_location}dimReasonForNewEpisode.csv")
+    legal_status = pd.read_csv(f"{output_location}dimLegalStatus.csv")
+    category_of_need = pd.read_csv(f"{output_location}dimCategoryOfNeed.csv")
+    placement_type = pd.read_csv(f"{output_location}dimPlacementType.csv")
+    placement_provider = pd.read_csv(f"{output_location}dimPlacementProvider.csv")
+    reason_episode_ceased = pd.read_csv(f"{output_location}dimReasonEpisodeCeased.csv")
+    reason_place_change = pd.read_csv(f"{output_location}dimReasonPlaceChange.csv")
+    postcode = pd.read_csv(f"{output_location}dimPostcode.csv")
+    ofsted_provider = pd.read_csv(f"{output_location}dimOfstedProvider.csv")
+    ons_area = pd.read_csv(f"{output_location}dimONSArea.csv")
+
+    # LookedAfterChildKey
+    episodes = episodes.merge(looked_after_child, left_on='CHILD', right_on='ChildIdentifier', how='left')
+
+    # ReasonForNewEpisodeKey
+    episodes = episodes.merge(reason_for_new_episode, left_on='RNE', right_on='ReasonForNewEpisodeCode', how='left')
+
+    # LegalStatusKey
+    episodes = episodes.merge(legal_status, left_on='LS', right_on='LegalStatusCode', how='left')
+
+    # CategoryOfNeedKey
+    episodes = episodes.merge(category_of_need, left_on='CIN', right_on='CategoryOfNeedCode', how='left')
+
+    # PlacementTypeKey
+    episodes = episodes.merge(placement_type, left_on='PLACE', right_on='PlacementTypeCode', how='left')
+
+    # PlacementProviderKey
+    episodes = episodes.merge(placement_provider, left_on='PLACE_PROVIDER', right_on='PlacementProviderCode', how='left')
+
+    # ReasonEpisodeCeasedKey
+    episodes = episodes.merge(reason_episode_ceased, left_on='REC', right_on='ReasonEpisodeCeasedCode', how='left')
+
+    # ReasonPlaceChangeKey
+    episodes = episodes.merge(reason_place_change, left_on='REASON_PLACE_CHANGE', right_on='ReasonPlaceChangeCode', how='left')
+
+    # OfstedProviderKey
+    ofsted_provider.URN = ofsted_provider.URN.astype(str)
+    episodes.URN = episodes.URN.astype(str)
+    episodes = episodes.merge(ofsted_provider, left_on='URN', right_on='URN', how='left')
+
+    # ONSAreaKey
+    episodes = episodes.merge(ons_area, left_on='LA', right_on='AreaName', how='left')
+
+    postcode = postcode[["PostcodeKey", "Sector"]]
+    # HomePostcodeKey
+    episodes = episodes.merge(postcode, left_on='HOME_POST', right_on='Sector', how='left')
+    episodes = episodes.rename(columns={"PostcodeKey": "HomePostcodeKey"})
+
+    # PlacementPostcodeKey
+    episodes = episodes.merge(postcode, left_on='PL_POST', right_on='Sector', how='left')
+    episodes = episodes.rename(columns={"PostcodeKey": "PlacementPostcodeKey"})
+
+    episodes.rename(columns=episodes_map, inplace=True)
+    episodes = episodes[["LookedAfterChildKey", "EpisodeCommencedDateKey", "ReasonForNewEpisodeKey", "LegalStatusKey", "CategoryOfNeedKey", "PlacementTypeKey", "PlacementProviderKey", "EpisodeCeasedDateKey",  "ReasonEpisodeCeasedKey", "ReasonPlaceChangeKey", "HomePostcodeKey", "PlacementPostcodeKey", "OfstedProviderKey", "ONSAreaKey", "SubmissionYearDateKey"]]
+
+    # any missing keys after merge should be replaced with -1
+    episode_key_columns = ["LookedAfterChildKey", "EpisodeCommencedDateKey", "ReasonForNewEpisodeKey", "LegalStatusKey", "CategoryOfNeedKey", "PlacementTypeKey", "PlacementProviderKey", "EpisodeCeasedDateKey",  "ReasonEpisodeCeasedKey", "ReasonPlaceChangeKey", "HomePostcodeKey", "PlacementPostcodeKey", "OfstedProviderKey", "ONSAreaKey", "SubmissionYearDateKey"]
+    episodes = fillna_categorical_columns(episodes, episode_key_columns)
+    
+    episodes.to_csv(f"{output_location}Output data\\factEpisode.csv", index=False)
+
+def create_factOfstedInspection():
+    ofsted_effectiveness = pd.read_csv(f'{output_location}dimOfstedEffectiveness.csv')
+    ofsted_provider = pd.read_csv(f'{output_location}dimOfstedProvider.csv')
+
+    provider_level_at_31Aug = pd.read_csv(f'{input_location_ext}Ofsted data\Provider_level_at_31_Aug_2023.csv')
+
+    # This sample file returned a UnicodeDecodeError so it was necessary to check that it is read with the right encoding type. 
+    # leaving in the safeguard until it works in production with the real file.
+    encoding = check_encoding(f'{input_location_ext}Ofsted data/Provider_level_in_year_2022-23.csv')
+    provider_level_in_year_2022_23 = pd.read_csv(f"{input_location_ext}Ofsted data/Provider_level_in_year_2022-23.csv", encoding=encoding)
+
+    # provider_level_in_year_2022_23 was observed to contain several unnamed empty columns.
+    unnamed_columns = [col for col in provider_level_in_year_2022_23.columns if 'Unnamed' in col]
+    provider_level_in_year_2022_23 = provider_level_in_year_2022_23.drop(columns=unnamed_columns)
+
+    # rename inspection date column in provider_level_at_31Aug so that they match when concatenated.
+    provider_level_at_31Aug = provider_level_at_31Aug.rename(columns={'Latest full inspection date': 'Inspection date',})
+    
+    factOfstedInspection = pd.concat([provider_level_in_year_2022_23, provider_level_at_31Aug])
+    factOfstedInspection = factOfstedInspection.drop_duplicates(subset=['URN', 'Inspection date'], keep='first')
+
+    # create IsLatest column that indicates if inspection is the most recent one recorded for a URN
+    factOfstedInspection["IsLatest"] = factOfstedInspection.groupby('URN')['Inspection date'].transform('max') == factOfstedInspection['Inspection date']
+
+    # Update the EndDate where isLatest is True with 2999 if EndDate is missing, otherwise keep it the same as InspectionDateKey
+    factOfstedInspection.loc[factOfstedInspection['IsLatest'] == True, 'EndDateKey'] = factOfstedInspection.loc[factOfstedInspection['IsLatest'] == True, 'Inspection date']
+    factOfstedInspection['EndDateKey'].fillna('2999-12-31', inplace=True)
+
+    # Find the next inspection date for each row where isLatest is False
+    next_inspection_dates = factOfstedInspection.loc[factOfstedInspection['IsLatest'] == False, 'Inspection date'].shift(-1)
+
+    # Update the EndDate where isLatest is False with the next inspection date
+    factOfstedInspection.loc[factOfstedInspection['IsLatest'] == False, 'EndDateKey'] = next_inspection_dates
+
+    factOfstedInspection = factOfstedInspection.rename(columns=inspection_map)
+    factOfstedInspection = factOfstedInspection[["InspectionDateKey", "EndDateKey", "OwnerName", "Effectiveness", "IsLatest"]]
+
+    factOfstedInspection.IsLatest = factOfstedInspection.IsLatest.map({True: "TRUE", False: "FALSE"})
+
+    # fill nans
+    categorical_columns = ["OwnerName"]
+    factOfstedInspection = fillna_categorical_columns(factOfstedInspection, categorical_columns)
+    date_columns = ["InspectionDateKey", "EndDateKey"]
+    factOfstedInspection = fillna_date_columns(factOfstedInspection, date_columns)
+    
+    # create OfstedEffectivenessKey
+    factOfstedInspection['Effectiveness'] = factOfstedInspection['Effectiveness'].fillna('Unknown')
+    factOfstedInspection = factOfstedInspection.merge(ofsted_effectiveness, how='left', left_on='Effectiveness', right_on='OverallEffectiveness')
+    factOfstedInspection = factOfstedInspection.drop(columns=['Effectiveness', 'OverallEffectiveness', 'Grade'])
+
+    # create OfstedProviderKey
+    ofsted_provider = ofsted_provider[['OfstedProviderKey', 'OwnerName']]
+    factOfstedInspection = factOfstedInspection.merge(ofsted_provider, how='left', on='OwnerName')
+    factOfstedInspection = factOfstedInspection.drop(columns=['OwnerName'])
+
+    # replace keys that couldn't be matched with -1
+    key_columns = ['OfstedProviderKey', 'OfstedEffectivenessKey']
+    factOfstedInspection = fillna_categorical_columns(factOfstedInspection, key_columns)
+
+    factOfstedInspection.reset_index(inplace=True, drop=True)
+    factOfstedInspection.reset_index(inplace=True, names='factOfstedInspectionKey')
+
+    factOfstedInspection.to_csv(f'{output_location}factOfstedInspection.csv', index=False)
+
+def create_sufficiency_data():
+    create_dim_tables()
+    create_dimONSArea()
+    create_dimLookedAfterChild()
+    create_dimOfstedProvider()
+    create_dimPostcode()
+    create_factEpisode()
     create_factOfstedInspection()
```

### Comparing `sufficiency_data_transform-0.1.0/sufficiency_data_transform/dim_maps.py` & `sufficiency_data_transform-0.1.1/sufficiency_data_transform/dim_maps.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,548 +1,548 @@
-category_of_need = [
-    {
-        "CategoryOfNeedKey": -1,
-        "CategoryOfNeedCode": -1,
-        "CategoryOfNeedDescription": "(Unknown)",
-    },
-    {
-        "CategoryOfNeedKey": 1,
-        "CategoryOfNeedCode": "N1",
-        "CategoryOfNeedDescription": "Abuse of neglect ",
-    },
-    {
-        "CategoryOfNeedKey": 2,
-        "CategoryOfNeedCode": "N2",
-        "CategoryOfNeedDescription": "Child's disability",
-    },
-    {
-        "CategoryOfNeedKey": 3,
-        "CategoryOfNeedCode": "N3",
-        "CategoryOfNeedDescription": "Parental illness or disability ",
-    },
-    {
-        "CategoryOfNeedKey": 4,
-        "CategoryOfNeedCode": "N4",
-        "CategoryOfNeedDescription": "Family in acute stress ",
-    },
-    {
-        "CategoryOfNeedKey": 5,
-        "CategoryOfNeedCode": "N5",
-        "CategoryOfNeedDescription": "Family dysfunction ",
-    },
-    {
-        "CategoryOfNeedKey": 6,
-        "CategoryOfNeedCode": "N6",
-        "CategoryOfNeedDescription": "Socially unacceptable behaviour ",
-    },
-    {
-        "CategoryOfNeedKey": 7,
-        "CategoryOfNeedCode": "N7",
-        "CategoryOfNeedDescription": "Low income ",
-    },
-    {
-        "CategoryOfNeedKey": 8,
-        "CategoryOfNeedCode": "N8",
-        "CategoryOfNeedDescription": "Absent parenting ",
-    },
-]
-
-legal_status = [
-    {
-        "LegalStatusKey": -1,
-        "LegalStatusCode": -1,
-        "LegalStatusDescription": "(Unknown)",
-    },
-    {
-        "LegalStatusKey": 1,
-        "LegalStatusCode": "C1",
-        "LegalStatusDescription": "Interim care order ",
-    },
-    {
-        "LegalStatusKey": 2,
-        "LegalStatusCode": "C2",
-        "LegalStatusDescription": "Full care order ",
-    },
-    {
-        "LegalStatusKey": 3,
-        "LegalStatusCode": "D1",
-        "LegalStatusDescription": "Freeing order granted ",
-    },
-    {
-        "LegalStatusKey": 4,
-        "LegalStatusCode": "E1",
-        "LegalStatusDescription": "Placement order granted ",
-    },
-    {
-        "LegalStatusKey": 5,
-        "LegalStatusCode": "J1",
-        "LegalStatusDescription": "Remanded to local authority accommodation or to youth detention accommodation ",
-    },
-    {
-        "LegalStatusKey": 6,
-        "LegalStatusCode": "J2",
-        "LegalStatusDescription": "Placed in local authority accommodation under the Police and Criminal Evidence Act 1984, including secure accommodation.  However, this would not necessarily be accommodation where the child would be detained. ",
-    },
-    {
-        "LegalStatusKey": 7,
-        "LegalStatusCode": "J3",
-        "LegalStatusDescription": "Sentenced to Youth Rehabilitation Order (Criminal Justice and Immigration Act 2008 as amended by Legal Aid, Sentencing and Punishment of Offenders Act (LASPOA) 2012 with residence or intensive fostering requirement) ",
-    },
-    {
-        "LegalStatusKey": 8,
-        "LegalStatusCode": "L1",
-        "LegalStatusDescription": "Under police protection and in local authority accommodation ",
-    },
-    {
-        "LegalStatusKey": 9,
-        "LegalStatusCode": "L2",
-        "LegalStatusDescription": "Emergency protection order (EPO) ",
-    },
-    {
-        "LegalStatusKey": 10,
-        "LegalStatusCode": "L3",
-        "LegalStatusDescription": "Under child assessment order and in local authority accommodation ",
-    },
-    {
-        "LegalStatusKey": 11,
-        "LegalStatusCode": "V2",
-        "LegalStatusDescription": "Single period of accommodation under section 20 (Children Act 1989) ",
-    },
-    {
-        "LegalStatusKey": 12,
-        "LegalStatusCode": "V3",
-        "LegalStatusDescription": "Accommodated under an agreed series of short-term breaks, when individual episodes of care are recorded ",
-    },
-    {
-        "LegalStatusKey": 13,
-        "LegalStatusCode": "V4",
-        "LegalStatusDescription": "Accommodated under an agreed series of short-term breaks, when agreements are recorded (NOT individual episodes of care) ",
-    },
-]
-
-ofsted_effectiveness = [
-    {"OfstedEffectivenessKey": -1, "Grade": -1, "OverallEffectiveness": "Unknown"},
-    {"OfstedEffectivenessKey": 1, "Grade": "4", "OverallEffectiveness": "Adequate"},
-    {
-        "OfstedEffectivenessKey": 2,
-        "Grade": "-",
-        "OverallEffectiveness": "Not provided as service is inspected as part of the ILACS inspection",
-    },
-    {
-        "OfstedEffectivenessKey": 3,
-        "Grade": "-",
-        "OverallEffectiveness": "Not yet inspected",
-    },
-    {"OfstedEffectivenessKey": 4, "Grade": "1", "OverallEffectiveness": "Outstanding"},
-    {"OfstedEffectivenessKey": 5, "Grade": "2", "OverallEffectiveness": "Good"},
-    {
-        "OfstedEffectivenessKey": 6,
-        "Grade": "3",
-        "OverallEffectiveness": "Requires improvement to be good",
-    },
-    {"OfstedEffectivenessKey": 7, "Grade": "5", "OverallEffectiveness": "Inadequate"},
-]
-
-placement_provider = [
-    {
-        "PlacementProviderKey": -1,
-        "PlacementProviderCode": -1,
-        "PlacementProviderDescription": "(Unknown)",
-    },
-    {
-        "PlacementProviderKey": 1,
-        "PlacementProviderCode": "PR0",
-        "PlacementProviderDescription": "Parent(s) or other person(s) with parental responsibility ",
-    },
-    {
-        "PlacementProviderKey": 2,
-        "PlacementProviderCode": "PR1",
-        "PlacementProviderDescription": "Own provision (by the local authority) including a regional adoption agency where the child's responsible local authority is the host authority ",
-    },
-    {
-        "PlacementProviderKey": 3,
-        "PlacementProviderCode": "PR2",
-        "PlacementProviderDescription": "Other local authority provision, including a regional adoption agency where another local authority is the host authority ",
-    },
-    {
-        "PlacementProviderKey": 4,
-        "PlacementProviderCode": "PR3",
-        "PlacementProviderDescription": "Other public provision (for example, a primary care trust) ",
-    },
-    {
-        "PlacementProviderKey": 5,
-        "PlacementProviderCode": "PR4",
-        "PlacementProviderDescription": "Private provision ",
-    },
-    {
-        "PlacementProviderKey": 6,
-        "PlacementProviderCode": "PR5",
-        "PlacementProviderDescription": "Voluntary/third sector provision ",
-    },
-]
-
-placement_type = [
-    {
-        "PlacementTypeKey": -1,
-        "PlacementTypeCode": -1,
-        "PlacementTypeDescription": "(Unknown)",
-    },
-    {
-        "PlacementTypeKey": 1,
-        "PlacementTypeCode": "A3",
-        "PlacementTypeDescription": "Placed for adoption with parental/guardian consent with current foster carer(s) (under Section 19 of the Adoption and Children Act 2002) or with a freeing order where parental/guardian consent has been given (under Section 18(1)(a) of the Adoption Act 1976) ",
-    },
-    {
-        "PlacementTypeKey": 2,
-        "PlacementTypeCode": "A4",
-        "PlacementTypeDescription": "Placed for adoption with parental/guardian consent not with current foster carer(s) (under Section 19 of the Adoption and Children Act 2002) or with a freeing order where parental/guardian consent has been given under Section 18(1)(a) of the Adoption Act 1976 ",
-    },
-    {
-        "PlacementTypeKey": 3,
-        "PlacementTypeCode": "A5",
-        "PlacementTypeDescription": "Placed for adoption with placement order with current foster carer(s) (under Section 21 of the Adoption and Children Act 2002) or with a freeing order where parental/guardian consent was dispensed with (under Section 18(1)(b) the Adoption Act 1976)",
-    },
-    {
-        "PlacementTypeKey": 4,
-        "PlacementTypeCode": "A6",
-        "PlacementTypeDescription": "Placed for adoption with placement order not with current foster carer(s) (under Section 21 of the Adoption and Children Act 2002) or with a freeing order where parental/guardian consent was dispensed with (under Section 18(1)(b) of the Adoption Act 1976) ",
-    },
-    {
-        "PlacementTypeKey": 5,
-        "PlacementTypeCode": "H5",
-        "PlacementTypeDescription": "Semi-independent living accommodation not subject to children's homes regulations ",
-    },
-    {
-        "PlacementTypeKey": 6,
-        "PlacementTypeCode": "K1",
-        "PlacementTypeDescription": "Secure children's homes ",
-    },
-    {
-        "PlacementTypeKey": 7,
-        "PlacementTypeCode": "K2",
-        "PlacementTypeDescription": "Children's Homes subject to Children's Homes Regulations ",
-    },
-    {
-        "PlacementTypeKey": 8,
-        "PlacementTypeCode": "P1",
-        "PlacementTypeDescription": "Placed with own parent(s) or other person(s) with parental responsibility ",
-    },
-    {
-        "PlacementTypeKey": 9,
-        "PlacementTypeCode": "P2",
-        "PlacementTypeDescription": "Independent living for example in a flat, lodgings, bedsit, bed and breakfast (B&B) or with friends, with or without formal support ",
-    },
-    {
-        "PlacementTypeKey": 10,
-        "PlacementTypeCode": "P3",
-        "PlacementTypeDescription": "Residential employment ",
-    },
-    {
-        "PlacementTypeKey": 11,
-        "PlacementTypeCode": "R1",
-        "PlacementTypeDescription": "Residential care home ",
-    },
-    {
-        "PlacementTypeKey": 12,
-        "PlacementTypeCode": "R2",
-        "PlacementTypeDescription": "National Health Service (NHS)/health trust or other establishment providing medical or nursing care ",
-    },
-    {
-        "PlacementTypeKey": 13,
-        "PlacementTypeCode": "R3",
-        "PlacementTypeDescription": "Family centre or mother and baby unit ",
-    },
-    {
-        "PlacementTypeKey": 14,
-        "PlacementTypeCode": "R5",
-        "PlacementTypeDescription": "Young offender institution (YOI) ",
-    },
-    {
-        "PlacementTypeKey": 15,
-        "PlacementTypeCode": "S1",
-        "PlacementTypeDescription": "All residential schools, except where dual-registered as a school and children's home ",
-    },
-    {
-        "PlacementTypeKey": 16,
-        "PlacementTypeCode": "T0",
-        "PlacementTypeDescription": "All types of temporary move (see paragraphs above for further details) ",
-    },
-    {
-        "PlacementTypeKey": 17,
-        "PlacementTypeCode": "T1",
-        "PlacementTypeDescription": "Temporary periods in hospital ",
-    },
-    {
-        "PlacementTypeKey": 18,
-        "PlacementTypeCode": "T2",
-        "PlacementTypeDescription": "Temporary absences of the child on holiday ",
-    },
-    {
-        "PlacementTypeKey": 19,
-        "PlacementTypeCode": "T3",
-        "PlacementTypeDescription": "Temporary accommodation whilst normal foster carer(s) is/are on holiday ",
-    },
-    {
-        "PlacementTypeKey": 20,
-        "PlacementTypeCode": "T4",
-        "PlacementTypeDescription": "Temporary accommodation of seven days or less, for any reason, not covered by codes T1 to T3 ",
-    },
-    {
-        "PlacementTypeKey": 21,
-        "PlacementTypeCode": "U1",
-        "PlacementTypeDescription": "Foster placement with relative(s) or friend(s) - long term fostering ",
-    },
-    {
-        "PlacementTypeKey": 22,
-        "PlacementTypeCode": "U2",
-        "PlacementTypeDescription": "Fostering placement with relative(s) or friend(s) who is/are also an approved adopter(s) - fostering for adoption /concurrent planning ",
-    },
-    {
-        "PlacementTypeKey": 23,
-        "PlacementTypeCode": "U3",
-        "PlacementTypeDescription": "Fostering placement with relative(s) or friend(s) who is/are not longterm or fostering for adoption /concurrent planning ",
-    },
-    {
-        "PlacementTypeKey": 24,
-        "PlacementTypeCode": "U4",
-        "PlacementTypeDescription": "Foster placement with other foster carer(s) - long term fostering ",
-    },
-    {
-        "PlacementTypeKey": 25,
-        "PlacementTypeCode": "U5",
-        "PlacementTypeDescription": "Foster placement with other foster carer(s) who is/are also an approved adopter(s) - fostering for adoption /concurrent planning ",
-    },
-    {
-        "PlacementTypeKey": 26,
-        "PlacementTypeCode": "U6",
-        "PlacementTypeDescription": "Foster placement with other foster carer(s) - not long term or fostering for adoption /concurrent planning ",
-    },
-    {
-        "PlacementTypeKey": 27,
-        "PlacementTypeCode": "Z1",
-        "PlacementTypeDescription": "Other placements (must be listed on a schedule sent to DfE with annual submission) ",
-    },
-]
-
-reason_episode_ceased = [
-    {
-        "ReasonEpisodeCeasedKey": -1,
-        "ReasonEpisodeCeasedCode": -1,
-        "ReasonEpisodeCeasedDescription": "(Unknown)",
-    },
-    {
-        "ReasonEpisodeCeasedKey": 1,
-        "ReasonEpisodeCeasedCode": "E11",
-        "ReasonEpisodeCeasedDescription": "Adopted - application for an adoption order unopposed   ",
-    },
-    {
-        "ReasonEpisodeCeasedKey": 2,
-        "ReasonEpisodeCeasedCode": "E12",
-        "ReasonEpisodeCeasedDescription": "Adopted - consent dispensed with by the court ",
-    },
-    {
-        "ReasonEpisodeCeasedKey": 3,
-        "ReasonEpisodeCeasedCode": "E13",
-        "ReasonEpisodeCeasedDescription": "Left care to live with parent(s), relative(s), or other person(s) with no parental responsibility. ",
-    },
-    {
-        "ReasonEpisodeCeasedKey": 4,
-        "ReasonEpisodeCeasedCode": "E14",
-        "ReasonEpisodeCeasedDescription": "Accommodation on remand ended ",
-    },
-    {
-        "ReasonEpisodeCeasedKey": 5,
-        "ReasonEpisodeCeasedCode": "E15",
-        "ReasonEpisodeCeasedDescription": "Age assessment determined child is aged 18 or over and E5, E6 and E7 do not apply, such as an unaccompanied asylum-seeking child (UASC) whose age has been disputed ",
-    },
-    {
-        "ReasonEpisodeCeasedKey": 6,
-        "ReasonEpisodeCeasedCode": "E16",
-        "ReasonEpisodeCeasedDescription": "Child moved abroad ",
-    },
-    {
-        "ReasonEpisodeCeasedKey": 7,
-        "ReasonEpisodeCeasedCode": "E17",
-        "ReasonEpisodeCeasedDescription": "Aged 18 (or over) and remained with current carers (inc under staying put arrangements) ",
-    },
-    {
-        "ReasonEpisodeCeasedKey": 8,
-        "ReasonEpisodeCeasedCode": "E2",
-        "ReasonEpisodeCeasedDescription": "Died ",
-    },
-    {
-        "ReasonEpisodeCeasedKey": 9,
-        "ReasonEpisodeCeasedCode": "E3",
-        "ReasonEpisodeCeasedDescription": "Care taken over by another local authority in the UK ",
-    },
-    {
-        "ReasonEpisodeCeasedKey": 10,
-        "ReasonEpisodeCeasedCode": "E41",
-        "ReasonEpisodeCeasedDescription": "Residence order (or, from 22 April 2014, a child arrangement order which sets out with whom the child is to live) granted ",
-    },
-    {
-        "ReasonEpisodeCeasedKey": 11,
-        "ReasonEpisodeCeasedCode": "E45",
-        "ReasonEpisodeCeasedDescription": "Special guardianship order made to former foster carer(s), who was/are a relative(s) or friend(s) ",
-    },
-    {
-        "ReasonEpisodeCeasedKey": 12,
-        "ReasonEpisodeCeasedCode": "E46",
-        "ReasonEpisodeCeasedDescription": "Special guardianship order made to former foster carer(s), other than relative(s) or friend(s) ",
-    },
-    {
-        "ReasonEpisodeCeasedKey": 13,
-        "ReasonEpisodeCeasedCode": "E47",
-        "ReasonEpisodeCeasedDescription": "Special guardianship order made to carer(s), other than former foster carer(s), who was/are a relative(s) or friend(s) ",
-    },
-    {
-        "ReasonEpisodeCeasedKey": 14,
-        "ReasonEpisodeCeasedCode": "E48",
-        "ReasonEpisodeCeasedDescription": "Special guardianship order made to carer(s), other than former foster carer(s), other than relative(s) or friend(s) ",
-    },
-    {
-        "ReasonEpisodeCeasedKey": 15,
-        "ReasonEpisodeCeasedCode": "E4A",
-        "ReasonEpisodeCeasedDescription": "Returned home to live with parent(s), relative(s), or other person(s) with parental responsibility as part of the care planning process (not under a special guardianship order or residence order or (from 22 April 2014) a child arrangement order). ",
-    },
-    {
-        "ReasonEpisodeCeasedKey": 16,
-        "ReasonEpisodeCeasedCode": "E4B",
-        "ReasonEpisodeCeasedDescription": "Returned home to live with parent(s), relative(s), or other person(s) with parental responsibility which was not part of the current care planning process (not under a special guardianship order or residence order or (from 22 April 2014) a child arrangement order). ",
-    },
-    {
-        "ReasonEpisodeCeasedKey": 17,
-        "ReasonEpisodeCeasedCode": "E5",
-        "ReasonEpisodeCeasedDescription": "Moved into independent living arrangement and no longer looked-after: supportive accommodation providing formalised advice/support arrangements (such as most hostels, young men's Christian association, foyers, staying close and care leavers projects). Includes both children leaving care before and at age 18 ",
-    },
-    {
-        "ReasonEpisodeCeasedKey": 18,
-        "ReasonEpisodeCeasedCode": "E6",
-        "ReasonEpisodeCeasedDescription": "Moved into independent living arrangement and no longer looked-after : accommodation providing no formalised advice/support arrangements (such as bedsit, own flat, living with friend(s)). Includes both children leaving care before and at age 18 ",
-    },
-    {
-        "ReasonEpisodeCeasedKey": 19,
-        "ReasonEpisodeCeasedCode": "E7",
-        "ReasonEpisodeCeasedDescription": "Transferred to residential care funded by adult social care services ",
-    },
-    {
-        "ReasonEpisodeCeasedKey": 20,
-        "ReasonEpisodeCeasedCode": "E8",
-        "ReasonEpisodeCeasedDescription": "Period of being looked-after ceased for any other reason (where none of the other reasons apply) ",
-    },
-    {
-        "ReasonEpisodeCeasedKey": 21,
-        "ReasonEpisodeCeasedCode": "E9",
-        "ReasonEpisodeCeasedDescription": "Sentenced to custody ",
-    },
-    {
-        "ReasonEpisodeCeasedKey": 22,
-        "ReasonEpisodeCeasedCode": "X1",
-        "ReasonEpisodeCeasedDescription": "Episode ceases, and new episode begins on same day, for any reason ",
-    },
-]
-
-reason_for_new_episode = [
-    {
-        "ReasonForNewEpisodeKey": -1,
-        "ReasonForNewEpisodeCode": -1,
-        "ReasonForNewEpisodeDescription": "(Unknown)",
-    },
-    {
-        "ReasonForNewEpisodeKey": 1,
-        "ReasonForNewEpisodeCode": "B",
-        "ReasonForNewEpisodeDescription": "Change of legal status and placement and carer(s) at the same time",
-    },
-    {
-        "ReasonForNewEpisodeKey": 2,
-        "ReasonForNewEpisodeCode": "L",
-        "ReasonForNewEpisodeDescription": "Change of legal status only",
-    },
-    {
-        "ReasonForNewEpisodeKey": 3,
-        "ReasonForNewEpisodeCode": "P",
-        "ReasonForNewEpisodeDescription": "Change of placement and carer(s) only",
-    },
-    {
-        "ReasonForNewEpisodeKey": 4,
-        "ReasonForNewEpisodeCode": "S",
-        "ReasonForNewEpisodeDescription": "Started to be looked-after",
-    },
-    {
-        "ReasonForNewEpisodeKey": 5,
-        "ReasonForNewEpisodeCode": "T",
-        "ReasonForNewEpisodeDescription": "Change of placement (but same carer(s)) only",
-    },
-    {
-        "ReasonForNewEpisodeKey": 6,
-        "ReasonForNewEpisodeCode": "U",
-        "ReasonForNewEpisodeDescription": "Change of legal status and change of placement (but same carer(s)) at the same time",
-    },
-]
-
-reason_place_change = [
-    {
-        "ReasonPlaceChangeKey": -1,
-        "ReasonPlaceChangeCode": -1,
-        "ReasonPlaceChangeDescription": "(Unknown)",
-    },
-    {
-        "ReasonPlaceChangeKey": 1,
-        "ReasonPlaceChangeCode": "ALLEG",
-        "ReasonPlaceChangeDescription": "Allegation (s47) ",
-    },
-    {
-        "ReasonPlaceChangeKey": 2,
-        "ReasonPlaceChangeCode": "APPRR",
-        "ReasonPlaceChangeDescription": "Approval removed ",
-    },
-    {
-        "ReasonPlaceChangeKey": 3,
-        "ReasonPlaceChangeCode": "CARPL",
-        "ReasonPlaceChangeDescription": "Change to/Implementation of Care Plan ",
-    },
-    {
-        "ReasonPlaceChangeKey": 4,
-        "ReasonPlaceChangeCode": "CHILD",
-        "ReasonPlaceChangeDescription": "Child requests placement end ",
-    },
-    {
-        "ReasonPlaceChangeKey": 5,
-        "ReasonPlaceChangeCode": "CLOSE",
-        "ReasonPlaceChangeDescription": "Resignation/ closure of provision ",
-    },
-    {
-        "ReasonPlaceChangeKey": 6,
-        "ReasonPlaceChangeCode": "CREQB",
-        "ReasonPlaceChangeDescription": "Carer(s) requests placement end due to child's behaviour ",
-    },
-    {
-        "ReasonPlaceChangeKey": 7,
-        "ReasonPlaceChangeCode": "CREQO",
-        "ReasonPlaceChangeDescription": "Carer(s) requests placement end other than due to child's behaviour ",
-    },
-    {
-        "ReasonPlaceChangeKey": 8,
-        "ReasonPlaceChangeCode": "CUSTOD",
-        "ReasonPlaceChangeDescription": "Custody arrangement ",
-    },
-    {
-        "ReasonPlaceChangeKey": 9,
-        "ReasonPlaceChangeCode": "LAREQ",
-        "ReasonPlaceChangeDescription": "Responsible/area authority requests placement end ",
-    },
-    {
-        "ReasonPlaceChangeKey": 10,
-        "ReasonPlaceChangeCode": "OTHER",
-        "ReasonPlaceChangeDescription": "Other ",
-    },
-    {
-        "ReasonPlaceChangeKey": 11,
-        "ReasonPlaceChangeCode": "PLACE",
-        "ReasonPlaceChangeDescription": "Change in the status of placement only ",
-    },
-    {
-        "ReasonPlaceChangeKey": 12,
-        "ReasonPlaceChangeCode": "STAND",
-        "ReasonPlaceChangeDescription": "Standards of care concern ",
-    },
-]
+category_of_need = [
+    {
+        "CategoryOfNeedKey": -1,
+        "CategoryOfNeedCode": -1,
+        "CategoryOfNeedDescription": "(Unknown)",
+    },
+    {
+        "CategoryOfNeedKey": 1,
+        "CategoryOfNeedCode": "N1",
+        "CategoryOfNeedDescription": "Abuse of neglect ",
+    },
+    {
+        "CategoryOfNeedKey": 2,
+        "CategoryOfNeedCode": "N2",
+        "CategoryOfNeedDescription": "Child's disability",
+    },
+    {
+        "CategoryOfNeedKey": 3,
+        "CategoryOfNeedCode": "N3",
+        "CategoryOfNeedDescription": "Parental illness or disability ",
+    },
+    {
+        "CategoryOfNeedKey": 4,
+        "CategoryOfNeedCode": "N4",
+        "CategoryOfNeedDescription": "Family in acute stress ",
+    },
+    {
+        "CategoryOfNeedKey": 5,
+        "CategoryOfNeedCode": "N5",
+        "CategoryOfNeedDescription": "Family dysfunction ",
+    },
+    {
+        "CategoryOfNeedKey": 6,
+        "CategoryOfNeedCode": "N6",
+        "CategoryOfNeedDescription": "Socially unacceptable behaviour ",
+    },
+    {
+        "CategoryOfNeedKey": 7,
+        "CategoryOfNeedCode": "N7",
+        "CategoryOfNeedDescription": "Low income ",
+    },
+    {
+        "CategoryOfNeedKey": 8,
+        "CategoryOfNeedCode": "N8",
+        "CategoryOfNeedDescription": "Absent parenting ",
+    },
+]
+
+legal_status = [
+    {
+        "LegalStatusKey": -1,
+        "LegalStatusCode": -1,
+        "LegalStatusDescription": "(Unknown)",
+    },
+    {
+        "LegalStatusKey": 1,
+        "LegalStatusCode": "C1",
+        "LegalStatusDescription": "Interim care order ",
+    },
+    {
+        "LegalStatusKey": 2,
+        "LegalStatusCode": "C2",
+        "LegalStatusDescription": "Full care order ",
+    },
+    {
+        "LegalStatusKey": 3,
+        "LegalStatusCode": "D1",
+        "LegalStatusDescription": "Freeing order granted ",
+    },
+    {
+        "LegalStatusKey": 4,
+        "LegalStatusCode": "E1",
+        "LegalStatusDescription": "Placement order granted ",
+    },
+    {
+        "LegalStatusKey": 5,
+        "LegalStatusCode": "J1",
+        "LegalStatusDescription": "Remanded to local authority accommodation or to youth detention accommodation ",
+    },
+    {
+        "LegalStatusKey": 6,
+        "LegalStatusCode": "J2",
+        "LegalStatusDescription": "Placed in local authority accommodation under the Police and Criminal Evidence Act 1984, including secure accommodation.  However, this would not necessarily be accommodation where the child would be detained. ",
+    },
+    {
+        "LegalStatusKey": 7,
+        "LegalStatusCode": "J3",
+        "LegalStatusDescription": "Sentenced to Youth Rehabilitation Order (Criminal Justice and Immigration Act 2008 as amended by Legal Aid, Sentencing and Punishment of Offenders Act (LASPOA) 2012 with residence or intensive fostering requirement) ",
+    },
+    {
+        "LegalStatusKey": 8,
+        "LegalStatusCode": "L1",
+        "LegalStatusDescription": "Under police protection and in local authority accommodation ",
+    },
+    {
+        "LegalStatusKey": 9,
+        "LegalStatusCode": "L2",
+        "LegalStatusDescription": "Emergency protection order (EPO) ",
+    },
+    {
+        "LegalStatusKey": 10,
+        "LegalStatusCode": "L3",
+        "LegalStatusDescription": "Under child assessment order and in local authority accommodation ",
+    },
+    {
+        "LegalStatusKey": 11,
+        "LegalStatusCode": "V2",
+        "LegalStatusDescription": "Single period of accommodation under section 20 (Children Act 1989) ",
+    },
+    {
+        "LegalStatusKey": 12,
+        "LegalStatusCode": "V3",
+        "LegalStatusDescription": "Accommodated under an agreed series of short-term breaks, when individual episodes of care are recorded ",
+    },
+    {
+        "LegalStatusKey": 13,
+        "LegalStatusCode": "V4",
+        "LegalStatusDescription": "Accommodated under an agreed series of short-term breaks, when agreements are recorded (NOT individual episodes of care) ",
+    },
+]
+
+ofsted_effectiveness = [
+    {"OfstedEffectivenessKey": -1, "Grade": -1, "OverallEffectiveness": "Unknown"},
+    {"OfstedEffectivenessKey": 1, "Grade": "4", "OverallEffectiveness": "Adequate"},
+    {
+        "OfstedEffectivenessKey": 2,
+        "Grade": "-",
+        "OverallEffectiveness": "Not provided as service is inspected as part of the ILACS inspection",
+    },
+    {
+        "OfstedEffectivenessKey": 3,
+        "Grade": "-",
+        "OverallEffectiveness": "Not yet inspected",
+    },
+    {"OfstedEffectivenessKey": 4, "Grade": "1", "OverallEffectiveness": "Outstanding"},
+    {"OfstedEffectivenessKey": 5, "Grade": "2", "OverallEffectiveness": "Good"},
+    {
+        "OfstedEffectivenessKey": 6,
+        "Grade": "3",
+        "OverallEffectiveness": "Requires improvement to be good",
+    },
+    {"OfstedEffectivenessKey": 7, "Grade": "5", "OverallEffectiveness": "Inadequate"},
+]
+
+placement_provider = [
+    {
+        "PlacementProviderKey": -1,
+        "PlacementProviderCode": -1,
+        "PlacementProviderDescription": "(Unknown)",
+    },
+    {
+        "PlacementProviderKey": 1,
+        "PlacementProviderCode": "PR0",
+        "PlacementProviderDescription": "Parent(s) or other person(s) with parental responsibility ",
+    },
+    {
+        "PlacementProviderKey": 2,
+        "PlacementProviderCode": "PR1",
+        "PlacementProviderDescription": "Own provision (by the local authority) including a regional adoption agency where the child's responsible local authority is the host authority ",
+    },
+    {
+        "PlacementProviderKey": 3,
+        "PlacementProviderCode": "PR2",
+        "PlacementProviderDescription": "Other local authority provision, including a regional adoption agency where another local authority is the host authority ",
+    },
+    {
+        "PlacementProviderKey": 4,
+        "PlacementProviderCode": "PR3",
+        "PlacementProviderDescription": "Other public provision (for example, a primary care trust) ",
+    },
+    {
+        "PlacementProviderKey": 5,
+        "PlacementProviderCode": "PR4",
+        "PlacementProviderDescription": "Private provision ",
+    },
+    {
+        "PlacementProviderKey": 6,
+        "PlacementProviderCode": "PR5",
+        "PlacementProviderDescription": "Voluntary/third sector provision ",
+    },
+]
+
+placement_type = [
+    {
+        "PlacementTypeKey": -1,
+        "PlacementTypeCode": -1,
+        "PlacementTypeDescription": "(Unknown)",
+    },
+    {
+        "PlacementTypeKey": 1,
+        "PlacementTypeCode": "A3",
+        "PlacementTypeDescription": "Placed for adoption with parental/guardian consent with current foster carer(s) (under Section 19 of the Adoption and Children Act 2002) or with a freeing order where parental/guardian consent has been given (under Section 18(1)(a) of the Adoption Act 1976) ",
+    },
+    {
+        "PlacementTypeKey": 2,
+        "PlacementTypeCode": "A4",
+        "PlacementTypeDescription": "Placed for adoption with parental/guardian consent not with current foster carer(s) (under Section 19 of the Adoption and Children Act 2002) or with a freeing order where parental/guardian consent has been given under Section 18(1)(a) of the Adoption Act 1976 ",
+    },
+    {
+        "PlacementTypeKey": 3,
+        "PlacementTypeCode": "A5",
+        "PlacementTypeDescription": "Placed for adoption with placement order with current foster carer(s) (under Section 21 of the Adoption and Children Act 2002) or with a freeing order where parental/guardian consent was dispensed with (under Section 18(1)(b) the Adoption Act 1976)",
+    },
+    {
+        "PlacementTypeKey": 4,
+        "PlacementTypeCode": "A6",
+        "PlacementTypeDescription": "Placed for adoption with placement order not with current foster carer(s) (under Section 21 of the Adoption and Children Act 2002) or with a freeing order where parental/guardian consent was dispensed with (under Section 18(1)(b) of the Adoption Act 1976) ",
+    },
+    {
+        "PlacementTypeKey": 5,
+        "PlacementTypeCode": "H5",
+        "PlacementTypeDescription": "Semi-independent living accommodation not subject to children's homes regulations ",
+    },
+    {
+        "PlacementTypeKey": 6,
+        "PlacementTypeCode": "K1",
+        "PlacementTypeDescription": "Secure children's homes ",
+    },
+    {
+        "PlacementTypeKey": 7,
+        "PlacementTypeCode": "K2",
+        "PlacementTypeDescription": "Children's Homes subject to Children's Homes Regulations ",
+    },
+    {
+        "PlacementTypeKey": 8,
+        "PlacementTypeCode": "P1",
+        "PlacementTypeDescription": "Placed with own parent(s) or other person(s) with parental responsibility ",
+    },
+    {
+        "PlacementTypeKey": 9,
+        "PlacementTypeCode": "P2",
+        "PlacementTypeDescription": "Independent living for example in a flat, lodgings, bedsit, bed and breakfast (B&B) or with friends, with or without formal support ",
+    },
+    {
+        "PlacementTypeKey": 10,
+        "PlacementTypeCode": "P3",
+        "PlacementTypeDescription": "Residential employment ",
+    },
+    {
+        "PlacementTypeKey": 11,
+        "PlacementTypeCode": "R1",
+        "PlacementTypeDescription": "Residential care home ",
+    },
+    {
+        "PlacementTypeKey": 12,
+        "PlacementTypeCode": "R2",
+        "PlacementTypeDescription": "National Health Service (NHS)/health trust or other establishment providing medical or nursing care ",
+    },
+    {
+        "PlacementTypeKey": 13,
+        "PlacementTypeCode": "R3",
+        "PlacementTypeDescription": "Family centre or mother and baby unit ",
+    },
+    {
+        "PlacementTypeKey": 14,
+        "PlacementTypeCode": "R5",
+        "PlacementTypeDescription": "Young offender institution (YOI) ",
+    },
+    {
+        "PlacementTypeKey": 15,
+        "PlacementTypeCode": "S1",
+        "PlacementTypeDescription": "All residential schools, except where dual-registered as a school and children's home ",
+    },
+    {
+        "PlacementTypeKey": 16,
+        "PlacementTypeCode": "T0",
+        "PlacementTypeDescription": "All types of temporary move (see paragraphs above for further details) ",
+    },
+    {
+        "PlacementTypeKey": 17,
+        "PlacementTypeCode": "T1",
+        "PlacementTypeDescription": "Temporary periods in hospital ",
+    },
+    {
+        "PlacementTypeKey": 18,
+        "PlacementTypeCode": "T2",
+        "PlacementTypeDescription": "Temporary absences of the child on holiday ",
+    },
+    {
+        "PlacementTypeKey": 19,
+        "PlacementTypeCode": "T3",
+        "PlacementTypeDescription": "Temporary accommodation whilst normal foster carer(s) is/are on holiday ",
+    },
+    {
+        "PlacementTypeKey": 20,
+        "PlacementTypeCode": "T4",
+        "PlacementTypeDescription": "Temporary accommodation of seven days or less, for any reason, not covered by codes T1 to T3 ",
+    },
+    {
+        "PlacementTypeKey": 21,
+        "PlacementTypeCode": "U1",
+        "PlacementTypeDescription": "Foster placement with relative(s) or friend(s) - long term fostering ",
+    },
+    {
+        "PlacementTypeKey": 22,
+        "PlacementTypeCode": "U2",
+        "PlacementTypeDescription": "Fostering placement with relative(s) or friend(s) who is/are also an approved adopter(s) - fostering for adoption /concurrent planning ",
+    },
+    {
+        "PlacementTypeKey": 23,
+        "PlacementTypeCode": "U3",
+        "PlacementTypeDescription": "Fostering placement with relative(s) or friend(s) who is/are not longterm or fostering for adoption /concurrent planning ",
+    },
+    {
+        "PlacementTypeKey": 24,
+        "PlacementTypeCode": "U4",
+        "PlacementTypeDescription": "Foster placement with other foster carer(s) - long term fostering ",
+    },
+    {
+        "PlacementTypeKey": 25,
+        "PlacementTypeCode": "U5",
+        "PlacementTypeDescription": "Foster placement with other foster carer(s) who is/are also an approved adopter(s) - fostering for adoption /concurrent planning ",
+    },
+    {
+        "PlacementTypeKey": 26,
+        "PlacementTypeCode": "U6",
+        "PlacementTypeDescription": "Foster placement with other foster carer(s) - not long term or fostering for adoption /concurrent planning ",
+    },
+    {
+        "PlacementTypeKey": 27,
+        "PlacementTypeCode": "Z1",
+        "PlacementTypeDescription": "Other placements (must be listed on a schedule sent to DfE with annual submission) ",
+    },
+]
+
+reason_episode_ceased = [
+    {
+        "ReasonEpisodeCeasedKey": -1,
+        "ReasonEpisodeCeasedCode": -1,
+        "ReasonEpisodeCeasedDescription": "(Unknown)",
+    },
+    {
+        "ReasonEpisodeCeasedKey": 1,
+        "ReasonEpisodeCeasedCode": "E11",
+        "ReasonEpisodeCeasedDescription": "Adopted - application for an adoption order unopposed   ",
+    },
+    {
+        "ReasonEpisodeCeasedKey": 2,
+        "ReasonEpisodeCeasedCode": "E12",
+        "ReasonEpisodeCeasedDescription": "Adopted - consent dispensed with by the court ",
+    },
+    {
+        "ReasonEpisodeCeasedKey": 3,
+        "ReasonEpisodeCeasedCode": "E13",
+        "ReasonEpisodeCeasedDescription": "Left care to live with parent(s), relative(s), or other person(s) with no parental responsibility. ",
+    },
+    {
+        "ReasonEpisodeCeasedKey": 4,
+        "ReasonEpisodeCeasedCode": "E14",
+        "ReasonEpisodeCeasedDescription": "Accommodation on remand ended ",
+    },
+    {
+        "ReasonEpisodeCeasedKey": 5,
+        "ReasonEpisodeCeasedCode": "E15",
+        "ReasonEpisodeCeasedDescription": "Age assessment determined child is aged 18 or over and E5, E6 and E7 do not apply, such as an unaccompanied asylum-seeking child (UASC) whose age has been disputed ",
+    },
+    {
+        "ReasonEpisodeCeasedKey": 6,
+        "ReasonEpisodeCeasedCode": "E16",
+        "ReasonEpisodeCeasedDescription": "Child moved abroad ",
+    },
+    {
+        "ReasonEpisodeCeasedKey": 7,
+        "ReasonEpisodeCeasedCode": "E17",
+        "ReasonEpisodeCeasedDescription": "Aged 18 (or over) and remained with current carers (inc under staying put arrangements) ",
+    },
+    {
+        "ReasonEpisodeCeasedKey": 8,
+        "ReasonEpisodeCeasedCode": "E2",
+        "ReasonEpisodeCeasedDescription": "Died ",
+    },
+    {
+        "ReasonEpisodeCeasedKey": 9,
+        "ReasonEpisodeCeasedCode": "E3",
+        "ReasonEpisodeCeasedDescription": "Care taken over by another local authority in the UK ",
+    },
+    {
+        "ReasonEpisodeCeasedKey": 10,
+        "ReasonEpisodeCeasedCode": "E41",
+        "ReasonEpisodeCeasedDescription": "Residence order (or, from 22 April 2014, a child arrangement order which sets out with whom the child is to live) granted ",
+    },
+    {
+        "ReasonEpisodeCeasedKey": 11,
+        "ReasonEpisodeCeasedCode": "E45",
+        "ReasonEpisodeCeasedDescription": "Special guardianship order made to former foster carer(s), who was/are a relative(s) or friend(s) ",
+    },
+    {
+        "ReasonEpisodeCeasedKey": 12,
+        "ReasonEpisodeCeasedCode": "E46",
+        "ReasonEpisodeCeasedDescription": "Special guardianship order made to former foster carer(s), other than relative(s) or friend(s) ",
+    },
+    {
+        "ReasonEpisodeCeasedKey": 13,
+        "ReasonEpisodeCeasedCode": "E47",
+        "ReasonEpisodeCeasedDescription": "Special guardianship order made to carer(s), other than former foster carer(s), who was/are a relative(s) or friend(s) ",
+    },
+    {
+        "ReasonEpisodeCeasedKey": 14,
+        "ReasonEpisodeCeasedCode": "E48",
+        "ReasonEpisodeCeasedDescription": "Special guardianship order made to carer(s), other than former foster carer(s), other than relative(s) or friend(s) ",
+    },
+    {
+        "ReasonEpisodeCeasedKey": 15,
+        "ReasonEpisodeCeasedCode": "E4A",
+        "ReasonEpisodeCeasedDescription": "Returned home to live with parent(s), relative(s), or other person(s) with parental responsibility as part of the care planning process (not under a special guardianship order or residence order or (from 22 April 2014) a child arrangement order). ",
+    },
+    {
+        "ReasonEpisodeCeasedKey": 16,
+        "ReasonEpisodeCeasedCode": "E4B",
+        "ReasonEpisodeCeasedDescription": "Returned home to live with parent(s), relative(s), or other person(s) with parental responsibility which was not part of the current care planning process (not under a special guardianship order or residence order or (from 22 April 2014) a child arrangement order). ",
+    },
+    {
+        "ReasonEpisodeCeasedKey": 17,
+        "ReasonEpisodeCeasedCode": "E5",
+        "ReasonEpisodeCeasedDescription": "Moved into independent living arrangement and no longer looked-after: supportive accommodation providing formalised advice/support arrangements (such as most hostels, young men's Christian association, foyers, staying close and care leavers projects). Includes both children leaving care before and at age 18 ",
+    },
+    {
+        "ReasonEpisodeCeasedKey": 18,
+        "ReasonEpisodeCeasedCode": "E6",
+        "ReasonEpisodeCeasedDescription": "Moved into independent living arrangement and no longer looked-after : accommodation providing no formalised advice/support arrangements (such as bedsit, own flat, living with friend(s)). Includes both children leaving care before and at age 18 ",
+    },
+    {
+        "ReasonEpisodeCeasedKey": 19,
+        "ReasonEpisodeCeasedCode": "E7",
+        "ReasonEpisodeCeasedDescription": "Transferred to residential care funded by adult social care services ",
+    },
+    {
+        "ReasonEpisodeCeasedKey": 20,
+        "ReasonEpisodeCeasedCode": "E8",
+        "ReasonEpisodeCeasedDescription": "Period of being looked-after ceased for any other reason (where none of the other reasons apply) ",
+    },
+    {
+        "ReasonEpisodeCeasedKey": 21,
+        "ReasonEpisodeCeasedCode": "E9",
+        "ReasonEpisodeCeasedDescription": "Sentenced to custody ",
+    },
+    {
+        "ReasonEpisodeCeasedKey": 22,
+        "ReasonEpisodeCeasedCode": "X1",
+        "ReasonEpisodeCeasedDescription": "Episode ceases, and new episode begins on same day, for any reason ",
+    },
+]
+
+reason_for_new_episode = [
+    {
+        "ReasonForNewEpisodeKey": -1,
+        "ReasonForNewEpisodeCode": -1,
+        "ReasonForNewEpisodeDescription": "(Unknown)",
+    },
+    {
+        "ReasonForNewEpisodeKey": 1,
+        "ReasonForNewEpisodeCode": "B",
+        "ReasonForNewEpisodeDescription": "Change of legal status and placement and carer(s) at the same time",
+    },
+    {
+        "ReasonForNewEpisodeKey": 2,
+        "ReasonForNewEpisodeCode": "L",
+        "ReasonForNewEpisodeDescription": "Change of legal status only",
+    },
+    {
+        "ReasonForNewEpisodeKey": 3,
+        "ReasonForNewEpisodeCode": "P",
+        "ReasonForNewEpisodeDescription": "Change of placement and carer(s) only",
+    },
+    {
+        "ReasonForNewEpisodeKey": 4,
+        "ReasonForNewEpisodeCode": "S",
+        "ReasonForNewEpisodeDescription": "Started to be looked-after",
+    },
+    {
+        "ReasonForNewEpisodeKey": 5,
+        "ReasonForNewEpisodeCode": "T",
+        "ReasonForNewEpisodeDescription": "Change of placement (but same carer(s)) only",
+    },
+    {
+        "ReasonForNewEpisodeKey": 6,
+        "ReasonForNewEpisodeCode": "U",
+        "ReasonForNewEpisodeDescription": "Change of legal status and change of placement (but same carer(s)) at the same time",
+    },
+]
+
+reason_place_change = [
+    {
+        "ReasonPlaceChangeKey": -1,
+        "ReasonPlaceChangeCode": -1,
+        "ReasonPlaceChangeDescription": "(Unknown)",
+    },
+    {
+        "ReasonPlaceChangeKey": 1,
+        "ReasonPlaceChangeCode": "ALLEG",
+        "ReasonPlaceChangeDescription": "Allegation (s47) ",
+    },
+    {
+        "ReasonPlaceChangeKey": 2,
+        "ReasonPlaceChangeCode": "APPRR",
+        "ReasonPlaceChangeDescription": "Approval removed ",
+    },
+    {
+        "ReasonPlaceChangeKey": 3,
+        "ReasonPlaceChangeCode": "CARPL",
+        "ReasonPlaceChangeDescription": "Change to/Implementation of Care Plan ",
+    },
+    {
+        "ReasonPlaceChangeKey": 4,
+        "ReasonPlaceChangeCode": "CHILD",
+        "ReasonPlaceChangeDescription": "Child requests placement end ",
+    },
+    {
+        "ReasonPlaceChangeKey": 5,
+        "ReasonPlaceChangeCode": "CLOSE",
+        "ReasonPlaceChangeDescription": "Resignation/ closure of provision ",
+    },
+    {
+        "ReasonPlaceChangeKey": 6,
+        "ReasonPlaceChangeCode": "CREQB",
+        "ReasonPlaceChangeDescription": "Carer(s) requests placement end due to child's behaviour ",
+    },
+    {
+        "ReasonPlaceChangeKey": 7,
+        "ReasonPlaceChangeCode": "CREQO",
+        "ReasonPlaceChangeDescription": "Carer(s) requests placement end other than due to child's behaviour ",
+    },
+    {
+        "ReasonPlaceChangeKey": 8,
+        "ReasonPlaceChangeCode": "CUSTOD",
+        "ReasonPlaceChangeDescription": "Custody arrangement ",
+    },
+    {
+        "ReasonPlaceChangeKey": 9,
+        "ReasonPlaceChangeCode": "LAREQ",
+        "ReasonPlaceChangeDescription": "Responsible/area authority requests placement end ",
+    },
+    {
+        "ReasonPlaceChangeKey": 10,
+        "ReasonPlaceChangeCode": "OTHER",
+        "ReasonPlaceChangeDescription": "Other ",
+    },
+    {
+        "ReasonPlaceChangeKey": 11,
+        "ReasonPlaceChangeCode": "PLACE",
+        "ReasonPlaceChangeDescription": "Change in the status of placement only ",
+    },
+    {
+        "ReasonPlaceChangeKey": 12,
+        "ReasonPlaceChangeCode": "STAND",
+        "ReasonPlaceChangeDescription": "Standards of care concern ",
+    },
+]
```

### Comparing `sufficiency_data_transform-0.1.0/sufficiency_data_transform/maps.py` & `sufficiency_data_transform-0.1.1/sufficiency_data_transform/maps.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-ethnic_description_map = {
-    "WBRI": "White British",
-    "WIRI": "White Irish",
-    "WOTH": "Any other White background",
-    "WIRT": "Traveller of Irish Heritage",
-    "GROM": "Gypsy/Roma",
-    "MWBC": "White and Black Caribbean",
-    "MWBA": "White and Black African",
-    "MWAS": "White and Asian",
-    "MOTH": "Any other Mixed background",
-    "AIND": "Indian",
-    "APKN": "Pakistani",
-    "ABAN": "Bangladeshi",
-    "CHNE": "Chinese",
-    "AOTH": "Any other Asian background",
-    "BCRB": "Caribbean",
-    "BAFR": "African",
-    "BOTH": "Any other Black background",
-    "OOTH": "Any other ethnic group",
-    "REFU": "Refused",
-    "NOBT": "Information not yet obtained",
-    "UNKNOWN": "Unknown",
-}
-
-uasc_status_map = {
-    0: "Child was not an unaccompanied asylum-seeking child (UASC) at any time during the year",
-    1: "Child was an unaccompanied asylum-seeking child (UASC) during the year",
-    "UNKNOWN": "Unknown",
-}
-
-category_of_need_map = {
-    "N1": "Abuse of neglect",
-    "N2": "Child's disability",
-    "N3": "Parental illness or disability",
-    "N4": "Family in acute stress",
-    "N5": "Family dysfunction",
-    "N6": "Socially unacceptable behaviour",
-    "N7": "Low income",
-    "N8": "Absent parenting",
-}
-postcodes_map = {
-    "pcd2": "Sector",
-    "oslaua": "ONSAreaCode",
-    "lsoa11": "LSOA2011",
-    "lat": "Latitude",
-    "long": "Longitude",
-    "oseast1m": "OSEastings",
-    "osnrth1m": "OSNorthings",
-    "imd": "IMD",
-}
-
-gender_map = {
-    1.0: "Male",
-    1: "Male",
-    2.0: "Female",
-    2: "Female",
-}
-
-ons_map = {
-    "_WD21CD": "WardCode",
-    "WD21NM": "WardName",
-    "LAD21CD": "LACode",
-    "LAD21NM": "LAName",
-    "CTY21CD": "CountyCode",
-    "CTY21NM": "CountyName",
-    "RGN21CD": "RegionCode",
-    "RGN21NM": "RegionName",
-    "CTRY21CD": "CountryCode",
-    "CTRY21NM": "CountryName",
-}
-
-dimLookedAfterChild_columns_map = {
-    "CHILD": "ChildIdentifier",
-    "SEX": "Gender",
-    "DOB": "DateOfBirthKey",
-    "ETHNIC": "EthnicCode",
-    "DUC": "UASCCeasedDateKey",
-    "YEAR": "SubmissionYearDateKey",
-}
-
-uasc_status_map = {
-    0: "Child was not an unaccompanied asylum-seeking child (UASC) at any time during the year",
-    1: "Child was an unaccompanied asylum-seeking child (UASC) during the year",
-    "UNKNOWN": "Unknown",
-}
-
-ofsted_provider_map = {
-    "Provision type": "ProviderType",
-    "Registration date": "RegistrationDate",
-    "Registration status": "ProviderStatus",
-    "Date closed": "ClosedDate",
-    "Places": "MaxUsers",
-    "Organisation name": "OwnerName",
-}
-
-ofsted_to_ons_map = {
-    "Westmorland and Furness": "Westmoreland",
-    "Bristol": "Bristol, City of",
-    "Bournemouth, Christchurch & Poole": "Bournemouth, Christchurch and Poole",
-    "Durham": "County Durham",
-    "Cumberland": "Carlisle",
-    "Herefordshire": "Herefordshire, County of",
-    "Kingston upon Hull": "Kingston upon Hull, City of",
-    "Southend on Sea": "Southend-on-Sea",
-}
-
-episodes_map = {"DECOM": "EpisodeCommencedDateKey",
-                "DEC": "EpisodeCeasedDateKey",
-                "YEAR": "SubmissionYearDateKey",
-                 }
-
-inspection_map = {"Inspection date": "InspectionDateKey",
-                  "Inspection publication date": "EndDateKey", # change
-                  "Organisation which owns the provider": "OwnerName", # to get OfstedProviderKey
-                  "Overall experiences and progress of children and young people": "Effectiveness", # to get OfstedEffectivenessKey
+ethnic_description_map = {
+    "WBRI": "White British",
+    "WIRI": "White Irish",
+    "WOTH": "Any other White background",
+    "WIRT": "Traveller of Irish Heritage",
+    "GROM": "Gypsy/Roma",
+    "MWBC": "White and Black Caribbean",
+    "MWBA": "White and Black African",
+    "MWAS": "White and Asian",
+    "MOTH": "Any other Mixed background",
+    "AIND": "Indian",
+    "APKN": "Pakistani",
+    "ABAN": "Bangladeshi",
+    "CHNE": "Chinese",
+    "AOTH": "Any other Asian background",
+    "BCRB": "Caribbean",
+    "BAFR": "African",
+    "BOTH": "Any other Black background",
+    "OOTH": "Any other ethnic group",
+    "REFU": "Refused",
+    "NOBT": "Information not yet obtained",
+    "UNKNOWN": "Unknown",
+}
+
+uasc_status_map = {
+    0: "Child was not an unaccompanied asylum-seeking child (UASC) at any time during the year",
+    1: "Child was an unaccompanied asylum-seeking child (UASC) during the year",
+    "UNKNOWN": "Unknown",
+}
+
+category_of_need_map = {
+    "N1": "Abuse of neglect",
+    "N2": "Child's disability",
+    "N3": "Parental illness or disability",
+    "N4": "Family in acute stress",
+    "N5": "Family dysfunction",
+    "N6": "Socially unacceptable behaviour",
+    "N7": "Low income",
+    "N8": "Absent parenting",
+}
+postcodes_map = {
+    "pcd2": "Sector",
+    "oslaua": "ONSAreaCode",
+    "lsoa11": "LSOA2011",
+    "lat": "Latitude",
+    "long": "Longitude",
+    "oseast1m": "OSEastings",
+    "osnrth1m": "OSNorthings",
+    "imd": "IMD",
+}
+
+gender_map = {
+    1.0: "Male",
+    1: "Male",
+    2.0: "Female",
+    2: "Female",
+}
+
+ons_map = {
+    "_WD21CD": "WardCode",
+    "WD21NM": "WardName",
+    "LAD21CD": "LACode",
+    "LAD21NM": "LAName",
+    "CTY21CD": "CountyCode",
+    "CTY21NM": "CountyName",
+    "RGN21CD": "RegionCode",
+    "RGN21NM": "RegionName",
+    "CTRY21CD": "CountryCode",
+    "CTRY21NM": "CountryName",
+}
+
+dimLookedAfterChild_columns_map = {
+    "CHILD": "ChildIdentifier",
+    "SEX": "Gender",
+    "DOB": "DateOfBirthKey",
+    "ETHNIC": "EthnicCode",
+    "DUC": "UASCCeasedDateKey",
+    "YEAR": "SubmissionYearDateKey",
+}
+
+uasc_status_map = {
+    0: "Child was not an unaccompanied asylum-seeking child (UASC) at any time during the year",
+    1: "Child was an unaccompanied asylum-seeking child (UASC) during the year",
+    "UNKNOWN": "Unknown",
+}
+
+ofsted_provider_map = {
+    "Provision type": "ProviderType",
+    "Registration date": "RegistrationDate",
+    "Registration status": "ProviderStatus",
+    "Date closed": "ClosedDate",
+    "Places": "MaxUsers",
+    "Organisation name": "OwnerName",
+}
+
+ofsted_to_ons_map = {
+    "Westmorland and Furness": "Westmoreland",
+    "Bristol": "Bristol, City of",
+    "Bournemouth, Christchurch & Poole": "Bournemouth, Christchurch and Poole",
+    "Durham": "County Durham",
+    "Cumberland": "Carlisle",
+    "Herefordshire": "Herefordshire, County of",
+    "Kingston upon Hull": "Kingston upon Hull, City of",
+    "Southend on Sea": "Southend-on-Sea",
+}
+
+episodes_map = {"DECOM": "EpisodeCommencedDateKey",
+                "DEC": "EpisodeCeasedDateKey",
+                "YEAR": "SubmissionYearDateKey",
+                 }
+
+inspection_map = {"Inspection date": "InspectionDateKey",
+                  "Inspection publication date": "EndDateKey", # change
+                  "Organisation which owns the provider": "OwnerName", # to get OfstedProviderKey
+                  "Overall experiences and progress of children and young people": "Effectiveness", # to get OfstedEffectivenessKey
                   }
```

### Comparing `sufficiency_data_transform-0.1.0/sufficiency_data_transform/utils.py` & `sufficiency_data_transform-0.1.1/sufficiency_data_transform/utils.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import chardet
-import pandas as pd
-
-def fillna_categorical_columns(df, columns):
-    """
-    Fill missing values in categorical columns with -1
-    """
-    for column in columns:
-        df[column] = df[column].fillna(-1)
-    return df
-
-def fillna_date_columns(df, columns):
-    """
-    Fill missing values in date columns with 2999-12-31
-    """
-    for column in columns:
-        df[column] = df[column].fillna('2999-12-31')
-    return df
-
-def check_encoding(file_path):
-    """
-    Check encoding of a file
-    """
-    with open(file_path, 'rb') as rawdata:
-        result = chardet.detect(rawdata.read())
-    return result['encoding']
-
-def add_nan_row(df, dfKey):
-    """
-    Add rows with NaN values in all the columns
-    """
-    # add a row that simulates the scenario where all values are nan
-    nan_col = {col:pd.NA for col in df.columns}
-    nan_col[dfKey] = -1
-    df.loc[len(df)] = nan_col
-    return df
-
-def generate_dim(data, filename):
-    pd.DataFrame(data).to_csv(filename, index=False)
-
-def check_encoding(file_path):
-    """
-    Check encoding of a file
-    """
-    with open(file_path, 'rb') as rawdata:
-        result = chardet.detect(rawdata.read())
+import chardet
+import pandas as pd
+
+def fillna_categorical_columns(df, columns):
+    """
+    Fill missing values in categorical columns with -1
+    """
+    for column in columns:
+        df[column] = df[column].fillna(-1)
+    return df
+
+def fillna_date_columns(df, columns):
+    """
+    Fill missing values in date columns with 2999-12-31
+    """
+    for column in columns:
+        df[column] = df[column].fillna('2999-12-31')
+    return df
+
+def check_encoding(file_path):
+    """
+    Check encoding of a file
+    """
+    with open(file_path, 'rb') as rawdata:
+        result = chardet.detect(rawdata.read())
+    return result['encoding']
+
+def add_nan_row(df, dfKey):
+    """
+    Add rows with NaN values in all the columns
+    """
+    # add a row that simulates the scenario where all values are nan
+    nan_col = {col:pd.NA for col in df.columns}
+    nan_col[dfKey] = -1
+    df.loc[len(df)] = nan_col
+    return df
+
+def generate_dim(data, filename):
+    pd.DataFrame(data).to_csv(filename, index=False)
+
+def check_encoding(file_path):
+    """
+    Check encoding of a file
+    """
+    with open(file_path, 'rb') as rawdata:
+        result = chardet.detect(rawdata.read())
     return result['encoding']
```

### Comparing `sufficiency_data_transform-0.1.0/PKG-INFO` & `sufficiency_data_transform-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: sufficiency-data-transform
-Version: 0.1.0
+Version: 0.1.1
 Summary: temp repo for liia sufficiency data transform
 License: MIT
 Author: tab1tha
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: chardet (>=5.2.0,<6.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: python-decouple (>=3.8,<4.0)
 Description-Content-Type: text/markdown
 
 This is a temporary repo that hosts code which needs to be plugged into the liia-tools-pipeline.
```

