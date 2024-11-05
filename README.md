# The CIRKULÆR Model Repository
Documentation regarding parameters and factors in the CIRKULÆR model

### Maintained by:
Henrik Thers, thers@agro.au.dk\
Jorge F. Miranda-Vélez, jorge_mv@agro.au.dk

Updates made to model parameters and assumptions will be published here.

Version 1.0 is used for the paper: <br/>
*The CIRKULÆR model – a national and regional static flow model of agricultural production, environmental and climatic impacts.\
Henrik Thers, Jorge Federico Miranda-Vélez, Lars Uldall-Jessen, Asbjørn Mølmer Sahlholdt, Mette Vestergaard Odgaard, August Kau Lægsgaard Madsen, Henrik Bjarne Møller, Peter Sørensen, Troels Kristensen*

**The following Excel books are available in order to document parameters, assumptions, and data sources.\
01_Parameter_input_CIRKULÆR_ver01\
02_Index_cards_Crops_and_related_tabels_ver01\
03_Index_cards_Technologies_and_related_tabels_ver01\
04_Index_cards_Livestock_and_related_tabels_ver01\
05_Index_cards_Manure_storage_Biogas_ver01**


## 01_Parameter_input_CIRKULÆR_ver01
The book is read by the model in the first module (Field) and the information is applied throughout the model.
The book contains a number of sheets in blue, which contain a number of data tables. The sheets are explained one by one below.
### Transportation:
Table 1 contains a list of the means of transportation that is available in the model.
### Emissions_and_deposition:
Table 2 lists the emission factors for direct nitrous oxide applied in the model.
Table 3 lists the emission factors for crop dependent ammonia.
Table 4 defines the atmospheric N deposition.
Table 5 lists the ratios between nitrous oxide and dinitrogen emissions for the soil categories included in the model.
### Organic soil emissions:
Table 6 lists the default greenhouse gas emission factors for soil containing 6-12 % and 12 % or more organic matter.
### Drying of harvest products:
Table 7 lists the energy consumption for drying of different categories of harvest products, e.g., grain.
In Table 8, the default moisture content at harvest for the above categories of harvest products are defined.
### Liming and soil C storage:
Table 9 defines the type and amount per hectare of lime that is assumed applied in the model.
Table 10. The model includes five carbon types, namely plant C, manure C, digested plant C, digested manure C and biochar C. Biochar C is treated separately. The first four are treated by recalculating them all into plant C. This is done by calculating a formular for conversion that includes the clay content of the soil. The formulars are present on this table. For further information see Appendix 1: Calculations of Plant-c-20y-equivalents.
Table 11 lists the assumed clay content for each of the six soil categories included in the model.
Table 12 provides formulars for calculation of soil C storage in a 20-years’ time perspective dependent on the clay content in each od the soil categories (from Table 11).
### GWP and indirect N2O:
Table 13 shows which set of global warming potentials and emission factors of indirect nitrous oxide from nitrate leaching and ammonia volatilization that are applied in the model. 

## 02_Index_cards_Crops_and_related_tabels_ver01
The book is associated with the Field module.
The book contains a number of sheets of which those with green shades define specific crops and those with blue shades contain associated information.
The first sheet, named Example, is yellow, and it explains the content of the crop index cards (green shades). It does so by using the crop Spring_barley_1 as an example. In the Example sheet, there has been a translation into English, and it is done in such way that the translation is always in the same cell as in the sheet Spring_barley_1. For instance, the text ‘Calculation of total crop fertilization’ in cell A27 in the Example sheet is the translation of the text in cell A27 in the Spring_barley_1 sheet. 
The index cards are made with a permanent part in grey shades and a fill-in-part in yellow cells. 
The additional information tables (sheets colored by blue shades) are explained one by one below.
The tables and their content are translated if needed, from the original table.
### Crop definitions: 
All products that can be grown in the Field module is created and defined in the main table (Table 18) of this sheet. The extent of the table covers from column A to X and continues from AC to AE. Each product is associated with a Biomass pool, which determines how the products will be pooled as the final part of the Field module. 
Table 19 in column Z-AA defines the overall proportion of nitrogen fertilizer application between conventional and organic agricultural systems.
### Imported products:
This sheet contains Table 20, which defines products that can be imported to the model. Besides the content definition, the table also holds information on emissions related to imported products. It is a choice in the model, whether these emissions should be included or not.
### Seed:
Table 21 contains the definitions of the seed that can be chosen in the index cards for crops.
Diesel consumption for field op(erations):
The different field operations that can be chosen in the crop index cards are listed (with English and Danish naming) together with their diesel consumption and the source (Table 22) (sources listed in Table 23). Some of the field operations need correction for soil type, due to that clay is heavier to cultivate than sand. The correction factors appear in Table 24 (together with factors for including lubrication oil).
### Other tables:
Product_groups and Destination groups are created in Table 25. 
In the major Table 26, the Biomass pools are created and linked to Product_groups and Destiny_groups. In addition, Biomass pools specific information is added, which includes information on volatile solids (manures have their volatile solids content calculated another place in the model), potential for biogas production, and principles for nitrogen, phosphorous and potassium utilization percentages, diesel consumption, and ammonia emissions when applied to the field.
In Table 27 the N, P, and K utilization percentages are defined for the included organic fertilizers.
In Table 28 the ammonia emissions from different application methods are defined.
In Table 29 a number of specific names/codes appears that can be included in a crop and/or sheet name, and which holds information that is used by the model.
### N fixation formula:
Contains information on parameters in the biological nitrogen fixation for a number of listed crops (Table 30). The calculations are available from the index cards.

## 03_Index_cards_Technologies_and_related_tabels_ver01
The book is associated with the Tech 1 and Tech 2 modules.
The book contains several sheets of which those with rose shades define specific technologies and the one with blue shade contains associated information, whereas the sheets with grey shade are copies from other Excel books and will only be explained briefly.
The first sheet, named Example, is yellow, and it explains the content of the technology index cards (rose shading). It does so by using the crop Pyrolysis_straw_conv as an example. In the Example sheet, there has been a translation into English, and it is done in such way that the translation is always in the same cell as in the sheet Pyrolysis_straw_conv. For instance, the text ‘Calculation of total crop fertilization’ in cells B 7-9 in the Example sheet is the translation of the text in cells B 7-9 in the Pyrolysis_straw_conv sheet. 
The index cards are made with a permanent part in grey shades and a fill-in-part in yellow cells. 
The additional information table (sheet in blue shade) and the grey copied sheets are explained one by one below.
The tables and their content are translated, if needed, from the original table.
### Processed products: 
All products in the model, emerging subsequently to the Field module, must be defined in one of the tables in this sheet. Defined products (Table 31) are those that always occur with a fixed content of C, N, P, K and MJ. 
Different types of energy produce can be defined in Table 32.
The undefined products (Table 33) may vary in C, N, P, K and MJ contents depending on the parental feedstock and flow paths that lead to the formation of the product. The table also holds information on how the content of volatile solids is quantified. In addition, several attributes for each undefined product are listed, regarding methane and other losses from stables and storage losses (except methane losses from storage, which is calculated in the Manure storage/biogas module).
### Biomass_pools_output_Field_modul:
Copy of the result output from the Field module, which lists the content of the Biomass pools that exists subsequently to the Field module. The information is needed in the TECH 1 module, when the biomass pools are treated in various technologies.
Biomass_pool_output_Biogas_Stor:
Copy of the result output from the Manure storage/Biogas module, which lists the content of the Biomass pools that exist subsequently to the Manure storage/Biogas module. The information is needed in the TECH 2 module, when the biomass pools are treated in various technologies.
### Crop definitions:
Copy of Table 18
### Imported products:
Copy of Table 20 
### Diesel consumption for field op:
Copy of Table 22
### Other_tables:
Mainly copies of Table 25 and the basic part of Table 26.

## 04_Index_cards_Livestock_and_related_tabels_ver01
The book is associated with the Livestock module.
The book contains several sheets of which those with green shades define specific technologies and the one with blue shade contain associated information, whereas the sheets with grey shade are copies from other Excel books and will only be explained briefly.
The first sheet, named Example, is yellow, and it explains the content of the livestock index cards (green shading). It does so by using the crop LittlePigs_up_to_31_1_conv as an example. In the Example sheet, there has been a translation into English, and it is done in such way that the translation is always in the same cell as in the sheet LittlePigs_up_to_31_1_conv. For instance, the text ‘Sum, adjustable protein + grain’ in cell F7 in the Example sheet is the translation of the text in cell F7 in the LittlePigs_up_to_31_1_conv sheet. 
The index cards are made with a permanent part in grey shades and a fill-in-part in yellow cells. 
The additional information table (sheet in blue shade) and the grey copied sheets are explained one by one below.
The tables and their content are translated, if needed, from the original table.
### Stable systems: 
A list of stable systems that can be selected for the livestock on the index cards are defined in Table 34. For each stable system, it is defined which manure types are produced and how the mass and content from the stable system (manure and bedding) are allocated to the manure types produced. Plant_C is a new attribute in the model, which shows the fraction of the manure that is plant material that has not been digested (bedding).
Table 35 contains information on default bedding quantities, so that it can easily be added to the index card.
### Converted_feedstuff:
Some feedstuffs are only processed if there is a need. That applies for instance to silage. When silage is used in a feed ration, the model calculates the losses associated with the ensiling process as well as the additional use of resources like diesel and plastic. Grass for grazing is another example, where losses are also calculated (due to grass trampling) and a negative use of diesel, because the default is that the grass is cut in the field, and thus, the model reverts the diesel consumption for this. Table 36 contains a list of feedstuffs that can be converted and the associated losses and resources.
### Respiration and enteric gas los(ses):
Enteric methane and associated losses for various livestock species is calculated according to the formulars in Table 37.
Respiration and associated losses for various livestock species is calculated according to the formulars in Table 38.
### Biomass_pool_output_Tech1_module:
Copy of the result output from the Tech 1 module, which lists the content of the Biomass pools that exists subsequently to the Tech 1 module. The information is needed in the Livestock module, when the biomass pools are treated in the feed rations defined in the index cards.
### Crop definitions:
Copy of Table 18
### Imported products:
Copy of Table 20 
### Diesel consumption for field op:
Copy of Table 22
### Other_tables:
Mainly copies of Table 25 and the basic part of Table 26.
### Processed products:
Copies of Table 31 and 32 and a reduced copy of Table 33.

## 05_Index_cards_Manure_storage_Biogas_ver01
The book is associated with the Manure storage/biogas module.
The book contains several sheets of which those with rose shades define pathways of storage and possibly anaerobic digestion and the sheets with grey shades are copies from other Excel books and will only be explained briefly.
The first sheet, named Example, is yellow, and it explains the content of the Manure storage/biogas index cards (rose shading). It does so by using the crop Sep_biogas_sep_catt_slurry_conv as an example. In the Example sheet, there has been a translation into English, and it is done in such way that the translation is always in the same cell as in the sheet Sep_biogas_sep_catt_slurry_conv. For instance, the text ‘Temperature for digestion” in cell F4 in the Example sheet is the translation of the text in cell F4 in the Sep_biogas_sep_catt_slurry_conv sheet. 
The index cards are made with a permanent part in grey shades and a fill-in-part in yellow cells. 
The grey copied sheets are explained one by one below.
### Biomass_pool_output_Livesto_mod:
Copy of the result output from the Livestock module, which lists the content of the Biomass pools that exist subsequently to the Livestock module. The information is needed in the Manure storage/biogas module, when the biomass pools are treated in the various pathways of storage and anaerobic digestion as defined in the index cards.
### Diesel consumption for field op:
Copy of Table 22
### Other_tables:
Mainly copies of Table 25 and the basic part of Table 26.
### Processed products:
Copies of Table 31 and 32 and a reduced copy of Table 33.
Converted_feedstuff:
Copy of Table 36.
