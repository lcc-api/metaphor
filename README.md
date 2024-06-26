# metaphor datasets
These dataset represent the efforts of Language Computer Corp. under the IARPA Metaphor Project from 2012-2014.
They are being released in two bundles -- a small version:
  
* en_small.xml (ENGLISH)	with  16265 source/target pairs, 17336 metaphoricity annotations, 7941 conceptual mapping annotations, and 3932 affect annotations
* es_small.xml (SPANISH)    with  14524 source/target pairs, 15743 metaphoricity annotations, 7365 conceptual mapping annotations, and 3569 affect annotations

and a large version:

* en_large.xml (ENGLISH)	with 167479 source/target pairs, 86860 metaphoricity annotations, 51324 conceptual mapping annotations, and 25277 affect annotations
* es_large.xml (SPANISH)    with 115799 source/target pairs, 70071 metaphoricity annotations, 46063 conceptual mapping annotations, and 21889 affect annotations
* ru_large.xml (RUSSIAN)	with  64019 source/target pairs, 48497 metaphoricity annotations, 24465 conceptual mapping annotations, and 13389 affect annotations
   fa_large.xml (FARSI)      with  80167 source/target pairs, 63750 metaphoricity annotations, 39529 conceptual mapping annotations, and 16953 affect annotations


These are released under the CreativeCommons-Attribution-NonCommercial-ShareAlike v4.0 license (https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode).

For all attribution, please cite (Mohler et al. 2016 -- Introducing the LCC Metaphor Datasets)

---

There are two associated xsd files -- large.xsd and small.xsd.

Attributes for the XML elements are defined as follows:

* annotatorID=`<NUMBER>`, uniquely identifying one of our annotators
* chain=`<SEQUENCE>`, indicating the relationhsip from the source to the target via prep-condensed MALT PARSER relations (with * indicating the common subsumer of source/target)
* creationTime=`<NUMBER>`, timestamp (ms) of annotation instance
* docid=`<NUMBER>`, uniquely identifying one of our documents
* id=`<NUMBER>`, uniquely identifying an annotation (of a particular type). Note that a MetaphoricityAnnotation and a PolarityAnnotation might have the same id.
* intensity=`<NUMBER>` (0, 1, 2, 3)
* polarity=`<VALUE>` (NEGATIVE, NEUTRAL, POSITIVE)
* protagonist=`<VALUE>` (GENERAL, GOVERNMENT_OVERSIGHT, INDIVIDUAL_OVERSIGHT)
* score=`<NUMBER>` (-1, 0, 1, 2, 3), where -1 indicates invalid syntactic relation between a source/target (only used for MetaphoricityAnnotations)
* sourceConcept=`<VALUE>`
>	ABYSS, ACCIDENT, ADDICTION, A_GOD, ANIMAL, A_RIGHT, AVERSION, BACKWARD_MOVEMENT, BARRIER, BATTLE, BLOOD_STREAM, BLOOD_SYSTEM, BODY_OF_WATER, BUILDING, BUSINESS, CLOTHING, COMPETITION, 
>	CONFINEMENT, CONTAINER, CONTAMINATION, CONTROL, CRIME, CROP, DARKNESS, DELICACY, DESIRE, DESTROYER, DISEASE, DOWNWARD_MOVEMENT, EMOTION_EXPERIENCER, EMPLOYEE, ENERGY, ENSLAVEMENT, FABRIC, 
>	FACTORY, FAMILY, FIRE, FOOD, FORCEFUL_EXTRACTION, FORWARD_MOVEMENT, FURNISHINGS, GAME, GAP, GEOGRAPHIC_FEATURE, GIFT, GOAL_DIRECTED, GOURMET_CUISINE, GREED, HAZARDOUS_GEOGRAPHIC_FEATURE, 
>	HIGH_LOCATION, HIGH_POINT, HUMAN_BODY, IMPURITY, INDUSTRY, INSANITY, JOURNEY, LEADER, LIFE_STAGE, LIGHT, LOW_LOCATION, LOW_POINT, MACHINE, MAGIC, MATERIAL, MAZE, MEDICINE, MONSTER, 
>	MORAL_DUTY, MOVEMENT, MOVEMENT_ON_A_VERTICAL_SCALE, NATURAL_PHYSICAL_FORCE, OBESITY, OBJECT_HANDLING, OTHER, PARASITE, PATHWAY, PHYSICAL_BURDEN, PHYSICAL_HARM, PHYSICAL_LOCATION, 
>	PHYSICAL_OBJECT, PLANT, PLIABILITY, PORTAL, POSITION_AND_CHANGE_OF_POSITION_ON_A_SCALE, PROTECTION, RACE, RESOURCE, RULE_ENFORCER, SCHISM, SCIENCE, SERVANT, SHAPE, SIZE, STAGE, STORY, 
> STRENGTH, STRUGGLE, TEMPERATURE, THEFT, TOOL, TRIBUTE, UPWARD_MOVEMENT, VEHICLE, VERTICAL_SCALE, VISION, WAR, WEAKNESS, WEATHER
* targetConcept=`<VALUE>`
>	ABORTION, BUREAUCRACY, CLIMATE_CHANGE, CONTROL_OF_GUNS, DEBT, DEMOCRACY, DEMOGRAPHICS, DISEASE, DRUG_TRAFFICKING, ELECTIONS, GOVERNMENT, GUN_DEBATE_GROUPS, GUN_OWNERSHIP, GUN_RIGHTS, GUNS, 
>	GUN_VIOLENCE, INTELLECTUAL_PROPERTY, ISLAMIC, MARRIAGE, MENTAL_CONCEPTS, MIGRATION, MONEY, NUCLEAR_WEAPONS, POLITICIANS, POVERTY, RELIGION, TAXATION, TAXES, TAXPAYERS, TERRORISM, WEALTH, 
>	WEAPONS_OF_MASS_DESTRUCTION, WELFARE
* type=`<VALUE>` (ANNOTATOR_EXAMPLES, RECALL_VALIDATIONS, SYSTEM_VALIDATIONS, UNVALIDATED)
