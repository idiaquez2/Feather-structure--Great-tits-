This README.GT.Colour.txt file was generated on 2023-04-26 by P. Salmón


GENERAL INFORMATION

1. Title of Dataset: Urbanisation impacts plumage colouration in a songbird across Europe: evidence from a correlational, experimental, and meta-analytical approach

2. Author Information
	A. Principal Investigator Contact Information
		Name: Pablo Salmón
		Institution: Institute of Avian Research "Vogelwarte Helgoland" (IAR)
		Address: An der Vogelwarte 21, 26386 Wilhelmshaven, Germany
		Email: pablo.salmon@ifv-vogelwarte.de

3. Date of data collection (single date, range, approximate date): 2014-04 to 2015-04

4. Geographic location of data collection: 10 populations across Europe (see methods)


DATA & FILE OVERVIEW

1. File List: 
 File #1- EU_GTcolour.csv - Data for the analysis of the 5 urban/forest pairs (adult birds) 
 File #2- cross_GTcolour.csv - Data for the nestling cross-fostering experiment between the urban and forest populations in Malmö
 File #3- Malmo_GTcolour.csv - Data for the cross-sectional data inr elation to age in the urban and forest populations in Malmö
 File #4- meta_GTcolour.csv - Data for the meta-analysis on great tit colouration response to urbanisation and pollution

2. Additional related data collected that was not included in the current data package: Adult birds body mass and tarsus; all ages Hue

3. Are there multiple versions of the dataset? No


METHODOLOGICAL INFORMATION

1. Description of methods used for collection/generation of data: 
Detailed methods in López-Idiáquez, D. et al. 2022, American Naturalist; Salmón, P. et al Nature communications, 12(1), 1-14.

2. Instrument- or software-specific information needed to interpret the data: All data were analysed in R (Version 4.1.1).

3. Describe any quality-assurance procedures performed on the data: 
Colouration was measured by a single person (D.L-I) with high repeatability across days. Chroma, adults: R= 0.85, 95%CI [0.697, 0.930]; nestlings: R= 0.79, 95%CI [0.525, 0.924]. Brightness, adults: R= 0.87, 95%CI [0.755, 0.939]; nestlings: R= 0.90, 95%CI [0.731, 0.965]; all p<0.001). See text for adjusted estimates.


DATA-SPECIFIC INFORMATION: EU_GTcolour.csv 

1. Number of variables: 9

2. Number of cases/rows:  1,428

3. Variable List (and units): 
	id = unique metal ring number or code (bird ID)
	samp_date = sampling date of the feather
	spectrum = spectrum ID
	YC = plumage chroma colouration (6 technical estimates per id)
	YB = plumage brightness (6 technical estimates per id)
	habitat = habitat where the bird was captured (Urban or Forest)
	area = Region for the urban-forest population pair. 5 levels that match with the name of the city (Lisbon, Madrid, Milan, Malmo and Gothenburg)
	sex = bird's sex. 1 = male; 2 = female
	age = bird's age. 1yr or 2yr+ 

	
4. Missing data code: n/a


DATA-SPECIFIC INFORMATION FOR: cross_GTcolour.csv

1. Number of variables: 12

2. Number of cases/rows:  523

3. Variable List (and units): 
	id = unique metal ring number or code (bird ID)
	samp_date = sampling date of the feather
	spectrum = spectrum ID
	YC = plumage chroma colouration (6 technical estimates per id)
	YB = plumage brightness (6 technical estimates per id)
	birthnest = nest ID of origin/birth
	rearnest = nest ID of rearing
	habitat_origin = habitat where the nest of birth was located (Urban or Forest)
	habitat_rearing = habitat where the nest of rearing was located (Urban or Forest)
    	cross_fostered = if the individual was cross-fostered or not (1 = yes, 0 = no)	
    	sex = bird's sex. 1 = male; 2 = female

4. Missing data code: n/a


DATA-SPECIFIC INFORMATION FOR: Malmo_GTcolour.csv

1. Number of variables: 9

2. Number of cases/rows:  1,140

3. Variable List (and units): 
	id = unique metal ring number or code (bird ID)
	samp_date = sampling date of the feather
	spectrum = spectrum ID
	YC = plumage chroma colouration (6 technical estimates per id)
	YB = plumage brightness (6 technical estimates per id) 
	habitat = habitat where the bird was captured (Urban or Forest)
	sex = bird's sex. 1 = male; 2 = female
	age = bird's age. nestling (15 days old), 1yr or 2yr+ 
	nest = nest ID where the bird was reared (nestling) or adults captured during breeding

4. Missing data code: n/a

5. Others: This data is a combination of File#1 (Malmo individuals) and File#2 


DATA-SPECIFIC INFORMATION FOR: meta_GTcolour.csv

1. Number of variables: 11

2. Number of cases/rows:  128

3. Variable List (and units): 
	Reference = Reference that the effect size was extracted from
	area = location of the study area, usually name of the closest city 
	disturbance = study on urbanisation or pollution
	sqrt_inv_eff_ss = small-study effect bias 
	sample_size = effect size sample size
	type = if the effect size on colouration comes from a mean comparison, 	"means" (urban area vs non-urban area; polluted area vs control) or from a 		correlation between urbanisation or pollution and colouration ("cors")
	obsID = effect size ID (for the residual variance)
	plumage_trait = type of colouration (3 levels see Table S3 in the supplementary 	material)
	life_stage = effect size from nestlings or adults
	COR_std = standardised effect size (correlation coefficient "r")
	COR_std_sv = standardised effect size variance

4. Missing data code: n/a in plumage traits specific to certain studies (effect sizes only used for the meta-analytical mean)