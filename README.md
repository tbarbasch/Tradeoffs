# Tradeoffs
Dataset for: Barbasch, T.A., Behrens, C., McLain, M., Arredondo, E., & Bell, A.M. A distinct neurogenomic response to a tradeoff between challenge and opportunity in male sticklebacks (_Gasterosteus aculeatus_). _Biology Letters._ Submitted.

# Methods
_Laboratory populations and housing_

All experiments were conducted during the summer breeding season (June – August) of 2020 using lab-reared individuals at the University of Illinois Urbana Champaign. Parents of the F1 individuals were wild caught from a population of the “white” ecotype (Blouw and Hagen 1990; Samuk 2016) of threespined stickleback (_Gasterosteus aculeatus_) from Canal Lake, Nova Scotia, CA. Laboratory conditions were maintained at 20 degrees C and a 16:8 light / dark photoperiod to stimulate male nesting behavior. All individuals were fed ad libitum once a day with a mixture of brine shrimp (Artemia sp.), mysis shrimp (Mysis sp.), bloodworms (Chironomus sp.), and Cyclop-Eeze. Prior to experimental trials, males and females were housed socially (5-20/tank, 53L x 33W x 24H cm), but focal males were moved to individual tanks at least 24 hours prior to experimental trials. N=17 focal males were used in this experiment.

_Experimental tank set-up_

Each experimental tank (53L x 33W x 24H cm) was filled with a layer of gravel on the bottom and divided into three sections. The middle section contained a clump of algae and a plastic tray filled with sand to provide nesting material, and the outer two sections were used to present stimuli during behavioral trials. To ensure construction of the nest in the middle section of the tank, the focal male was first confined to the middle section using dividers. After the nest was constructed, the dividers were removed so trials could be conducted.

_Overview of behavioral trials_

Behavioral trials were conducted in August 2020 to investigate the behavioral mechanisms underlying how males managed the competing demands of courtship and territory defense. Behavioral trials consisted of four different treatments: a courtship opportunity, a territorial challenge, simultaneous courtship opportunity and territorial challenge (hereafter referred to as the “tradeoff” treatment), and a control. At the start of each trial, two flasks were introduced into the focal male’s tank. In the courtship opportunity treatment, a gravid female was confined to one of the flasks (the other flask was empty), in the territorial challenge treatment, a rival male (a male displaying breeding coloration) was confined to one of the flasks, and in the tradeoff treatment, a gravid female was confined to one of the flasks and a rival male was confined to the other flask. Rival males were size matched to focal males as much as possible, which gave an average ratio of intruder standard length to focal standard length of 0.97mm (+/- 0.02 standard deviation). In the control treatment, males were presented with two empty flasks. Each focal male was exposed to each of the four treatments (courtship opportunity, territorial challenge, tradeoff, and control) twice in a randomized block design, for a total of eight trials per focal male. Therefore, each focal male was exposed to each of the four treatments in a random order once, followed by each of the four treatments in a random order a second time. Each male was exposed to only one trial per day. 

The focal male was acclimated to the presence of the observer for five minutes before the start of each trial. For each trial, the side of the tank where the flask containing a stimulus was placed was determined by coin toss (excepting the control treatment, which consisted of an empty flask on each side). The two flasks were then gently placed on their respective sides of the tank and male behavior was scored for five minutes using JWatcher (Blumstein and Daniel 2007). The number of zigzag displays (a courtship display) and the number of bites performed by the male were recorded.

_RNA extraction and sequencing_

Sixty minutes after their final trial (n=4 males after a courtship opportunity, n=5 males after a territorial intrusion, n=4 males after the tradeoff treatment, and n=4 males after the control treatment), the diencephalon and telencephalon were rapidly dissected, preserved in RNAlater, and deep frozen at -80 degrees C until extraction. RNA was extracted using Invitrogen PureLink RNA extraction kits (Invitrogen Corporation, Carlsbad, CA) and quality was checked using Agilent Bioanalyzer chips. Sequencing was performed by the Functional Genomics Unit of the W.M. Keck Center (University of Illinois Urbana Champaign). Libraries were prepped using TruSeq Stranded mRNA sample prep kits and samples were sequenced to a depth of >30M reads on a Novaseq 6000 S4 flow cell (Illumina). Reads were aligned to the stickleback reference genome (Ensembl release 95; Jones et al. 2012; Nath et al. 2021; Peichel et al. 2020) using STAR (Dobin et al. 2013) and read counts generated using HTSeq (Anders et al. 2015).

# Behavioral Data: 2020Tradeoffs.csv

_Description of Variables_

date: Calendar date that data was collected

ID: Unique identifier for each focal male

time: Time at the start of the trial

bites: Number of bites performed by the focal male during the 5 minute trial

zigzags: Number of zigzags performed by the focal male during the 5 minute trial

Treatment: Treatment the male was given. M = Territorial challenge, F = Courtship Opportunity, MF = Tradeoff, C = Control

Trial set: Whether the trial occurred during the first or second time the set of four trials was presented

Trial order: Whether the stimulus was presented first, second, third, or fourth in the sequence

# Sample Info: Aggression_sampleinfo.csv

_Description of Variables_

Sample: Unique identifier for each brain sample

ExtractionDate: Calendar date when brain sample was taken

Population: Identifier for the stickleback population from which data were taken

Family: ID number of family that male originated from

Experiment: Identifier for which experiment the samples belong

Treatment: Treatment the male was given (as with Behavioral Data)

bites: Number of bites performed by the focal male during the last trial before brain dissection

zigzags: Number of zigzags performed by the focal male during the last trial before brain dissection

# htseq_results

Count data from diencephalon

# htseq_T_results

Count data from telencephalon

# eFDR_null_pvalues

null distribution of p-values for eFDR correction

# eFDR_contrast_pvalues

eFDR corrected p-values

