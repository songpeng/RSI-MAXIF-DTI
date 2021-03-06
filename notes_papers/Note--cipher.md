##Cipher for identifying drug targets
(papaer:network-based relating pharmacological and genomic spaces for drug target identification)\




####predecessors theories
methods:use both **chemical similarity** and **phenotypic index** in parmacological space and prot-prot connection

results:speed identificatino of drug target 
        new applications and side effect for existing drugs

*phenotypic effect-based approach*is based on responses to external compounds

*chemical structure-based approach* integrates drug chemical similarity and protein sequence/structure information

**assumption and prediction**

structurally similar drugs tend to bind similar protein 

so associated drug pairs tend to have same targets and then the new drug-target interaction was predicted out

####challenges
1.similar responses may due to similar pathway or biological process instead of same target

2.expression pattern could not distinguish target from downstream genes(which may also response to external compounds?)

3.lack of prior information for major chemicals and proteins

4.assumption is wrong: many similar drugs bind different sequence or structure proteins

5.clear boundary between two methods

####drugCipher

PPI:prot-prot interaction

TS:drug therapeutic simmilarity

CS:drug chemical similarity

ATC: anatomic therapeutic chemical classification system(resources of TS)

MS:multiple similarity combine TS and CS

HPRD:human protein reference database

we get TS and CS two sets for drug 'd' to form pharmacological space between d and drug seeds and one closeness(associate d with arbitrary protein) for drug-target protein. Concordance score computed based on three linear regression models between TS-fi,CS-fi,TS-CS-fi.(assume linear relation between three) and this score represents the intensity of the connection.


####comparison between pharmacological metrics and genomic metrics

genomic space--GR--defined by average closeness--fi--protein character

pharmacological space--TS & CS--drug character

shows no absolute relation between GR CS TS



####performance of drugCipher

**precision**-- proportion of success(known target was ranked at the top )--cipher MS highest 

**sensitivity and specificity**--cipher ms highest

**proportion of identifying interaction** -- cipher ms highest


####compare with other methods

previous---limited number of proteins    no quantitative results 

BLM--one of most precise--average performance of BLM by weight of number of corresponding interactions is much lower than cipher ms



####Conclusion

integration of multi dimensional information gains advantages in target identification and yields additional knowledge associating drugs with diseases and pathways predicting new applications of drug side effects.


