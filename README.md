# 2KUROPS
DNA methylation to create heat maps

# select data that corresponds to methylation state at CpG islands near BMP6 gene
# remove any lines with "NA" for betamethylation value
grep -w "BMP6" 02met.txt | grep -vw "NA" 02met.txt > 0BMP6.txt
grep -w "BMP6" 02met.txt | grep -vw "NA" 02met.txt > 0BMP6.txt
grep -w "BMP6" 03met.txt | grep -vw "NA" 02met.txt > 03BMP6.txt
grep -w "BMP6" 04met.txt | grep -vw "NA" 02met.txt > 04BMP6.txt
grep -w "BMP6" 05met.txt | grep -vw "NA" 02met.txt > 05BMP6.txt
grep -w "BMP6" 06met.txt | grep -vw "NA" 02met.txt > 06BMP6.txt
grep -w "BMP6" 07met.txt | grep -vw "NA" 02met.txt > 07BMP6.txt
grep -w "BMP6" 08met.txt | grep -vw "NA" 02met.txt > 08BMP6.txt
grep -w "BMP6" 09met.txt | grep -vw "NA" 02met.txt > 09BMP6.txt
grep -w "BMP6" 10met.txt | grep -vw "NA" 02met.txt > 10BMP6.txt
grep -w "BMP6" 11met.txt | grep -vw "NA" 02met.txt > 11BMP6.txt
grep -w "BMP6" 12met.txt | grep -vw "NA" 02met.txt > 12BMP6.txt
grep -w "BMP6" 13met.txt | grep -vw "NA" 02met.txt > 13BMP6.txt
grep -w "BMP6" 14met.txt | grep -vw "NA" 02met.txt > 14BMP6.txt
grep -w "BMP6" 15met.txt | grep -vw "NA" 02met.txt > 15BMP6.txt
grep -w "BMP6" 16met.txt | grep -vw "NA" 02met.txt > 16BMP6.txt
grep -w "BMP6" 17met.txt | grep -vw "NA" 02met.txt > 17BMP6.txt
grep -w "BMP6" 18met.txt | grep -vw "NA" 02met.txt > 18BMP6.txt
grep -w "BMP6" 19met.txt | grep -vw "NA" 02met.txt > 19BMP6.txt
grep -w "BMP6" 20met.txt | grep -vw "NA" 02met.txt > 20BMP6.txt
grep -w "BMP6" 21met.txt | grep -vw "NA" 02met.txt > 21BMP6.txt
grep -w "BMP6" 22met.txt | grep -vw "NA" 02met.txt > 22BMP6.txt
grep -w "BMP6" 23met.txt | grep -vw "NA" 02met.txt > 23BMP6.txt
grep -w "BMP6" 24met.txt | grep -vw "NA" 02met.txt > 24BMP6.txt
grep -w "BMP6" 25met.txt | grep -vw "NA" 02met.txt > 25BMP6.txt
grep -w "BMP6" 26met.txt | grep -vw "NA" 02met.txt > 26BMP6.txt
grep -w "BMP6" 27met.txt | grep -vw "NA" 02met.txt > 27BMP6.txt
grep -w "BMP6" 28met.txt | grep -vw "NA" 02met.txt > 28BMP6.txt
grep -w "BMP6" 29met.txt | grep -vw "NA" 02met.txt > 29BMP6.txt
grep -w "BMP6" 30met.txt | grep -vw "NA" 02met.txt > 30BMP6.txt
grep -w "BMP6" 31met.txt | grep -vw "NA" 02met.txt > 31BMP6.txt
grep -w "BMP6" 32met.txt | grep -vw "NA" 02met.txt > 32BMP6.txt
grep -w "BMP6" 33met.txt | grep -vw "NA" 02met.txt > 33BMP6.txt
grep -w "BMP6" 34met.txt | grep -vw "NA" 02met.txt > 34BMP6.txt
grep -w "BMP6" 35met.txt | grep -vw "NA" 02met.txt > 35BMP6.txt
grep -w "BMP6" 36met.txt | grep -vw "NA" 02met.txt > 36BMP6.txt
grep -w "BMP6" 37met.txt | grep -vw "NA" 02met.txt > 37BMP6.txt
grep -w "BMP6" 38met.txt | grep -vw "NA" 02met.txt > 38BMP6.txt
grep -w "BMP6" 39met.txt | grep -vw "NA" 02met.txt > 39BMP6.txt
grep -w "BMP6" 40met.txt | grep -vw "NA" 02met.txt > 40BMP6.txt
grep -w "BMP6" 41met.txt | grep -vw "NA" 02met.txt > 41BMP6.txt
grep -w "BMP6" 42met.txt | grep -vw "NA" 02met.txt > 42BMP6.txt
grep -w "BMP6" 43met.txt | grep -vw "NA" 02met.txt > 43BMP6.txt
grep -w "BMP6" 44met.txt | grep -vw "NA" 02met.txt > 44BMP6.txt
grep -w "BMP6" 45met.txt | grep -vw "NA" 02met.txt > 45BMP6.txt
grep -w "BMP6" 46met.txt | grep -vw "NA" 02met.txt > 46BMP6.txt
grep -w "BMP6" 47met.txt | grep -vw "NA" 02met.txt > 47BMP6.txt

# filter for betamethylation values within the 2kb window
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 01BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 01BMP6.txt > 01BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 02BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 02BMP6.txt > 02BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 03BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 03BMP6.txt > 03BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 04BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 04BMP6.txt > 04BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 05BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 05BMP6.txt > 05BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 06BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 06BMP6.txt > 06BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 07BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 07BMP6.txt > 07BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 08BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 08BMP6.txt > 08BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 09BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 09BMP6.txt > 09BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 10BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 10BMP6.txt > 10BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 11BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 11BMP6.txt > 11BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 12BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 12BMP6.txt > 12BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 13BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 13BMP6.txt > 13BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 14BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 14BMP6.txt > 14BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 15BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 15BMP6.txt > 15BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 16BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 16BMP6.txt > 16BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 17BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 17BMP6.txt > 17BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 18BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 18BMP6.txt > 18BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 19BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 19BMP6.txt > 19BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 20BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 20BMP6.txt > 20BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 21BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 21BMP6.txt > 21BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 22BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 22BMP6.txt > 22BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 23BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 23BMP6.txt > 23BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 24BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 24BMP6.txt > 24BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 25BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 25BMP6.txt > 25BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 26BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 26BMP6.txt > 26BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 27BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 27BMP6.txt > 27BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 28BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 28BMP6.txt > 28BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 29BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 29BMP6.txt > 29BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 30BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 30BMP6.txt > 30BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 31BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 31BMP6.txt > 31BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 32BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 32BMP6.txt > 32BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 33BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 33BMP6.txt > 33BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 34BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 34BMP6.txt > 34BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 35BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 35BMP6.txt > 35BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 36BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 36BMP6.txt > 36BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 37BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 37BMP6.txt > 37BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 38BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 38BMP6.txt > 38BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 39BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 39BMP6.txt > 39BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 40BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 40BMP6.txt > 40BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 41BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 41BMP6.txt > 41BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 42BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 42BMP6.txt > 42BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 43BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 43BMP6.txt > 43BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 44BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 44BMP6.txt > 44BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 45BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 45BMP6.txt > 45BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 46BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 46BMP6.txt > 46BMP6filt.txt
awk '{if ($4>7726011) print $1,$2,$3,$4,$5}' 47BMP6.txt | awk '{if ($4<7728011) print $1,$2,$3,$4,$5}' 47BMP6.txt > 47BMP6filt.txt

# combine all data into one single txt file
## $2 = Betamethylation value
## $1 = CG probe ID
## $3 = Chromosome number
## $4 = Probe start
awk '{print $1,$3,$4,$2}' 01BMP6filt.txt > 01BMP6meth.txt
awk '{print $2}' 02BMP6filt.txt > 02BMP6meth.txt
awk '{print $2}' 03BMP6filt.txt > 03BMP6meth.txt
awk '{print $2}' 04BMP6filt.txt > 04BMP6meth.txt
awk '{print $2}' 05BMP6filt.txt > 05BMP6meth.txt
awk '{print $2}' 06BMP6filt.txt > 06BMP6meth.txt
awk '{print $2}' 07BMP6filt.txt > 07BMP6meth.txt
awk '{print $2}' 08BMP6filt.txt > 08BMP6meth.txt
awk '{print $2}' 09BMP6filt.txt > 09BMP6meth.txt
awk '{print $2}' 10BMP6filt.txt > 10BMP6meth.txt
awk '{print $2}' 11BMP6filt.txt > 11BMP6meth.txt
awk '{print $2}' 12BMP6filt.txt > 12BMP6meth.txt
awk '{print $2}' 13BMP6filt.txt > 13BMP6meth.txt
awk '{print $2}' 14BMP6filt.txt > 14BMP6meth.txt
awk '{print $2}' 15BMP6filt.txt > 15BMP6meth.txt
awk '{print $2}' 16BMP6filt.txt > 16BMP6meth.txt
awk '{print $2}' 17BMP6filt.txt > 17BMP6meth.txt
awk '{print $2}' 18BMP6filt.txt > 18BMP6meth.txt
awk '{print $2}' 19BMP6filt.txt > 19BMP6meth.txt
awk '{print $2}' 20BMP6filt.txt > 20BMP6meth.txt
awk '{print $2}' 21BMP6filt.txt > 21BMP6meth.txt
awk '{print $2}' 22BMP6filt.txt > 22BMP6meth.txt
awk '{print $2}' 23BMP6filt.txt > 23BMP6meth.txt
awk '{print $2}' 24BMP6filt.txt > 24BMP6meth.txt
awk '{print $2}' 25BMP6filt.txt > 25BMP6meth.txt
awk '{print $2}' 26BMP6filt.txt > 26BMP6meth.txt
awk '{print $2}' 27BMP6filt.txt > 27BMP6meth.txt
awk '{print $2}' 28BMP6filt.txt > 28BMP6meth.txt
awk '{print $2}' 29BMP6filt.txt > 29BMP6meth.txt
awk '{print $2}' 30BMP6filt.txt > 30BMP6meth.txt
awk '{print $2}' 31BMP6filt.txt > 31BMP6meth.txt
awk '{print $2}' 32BMP6filt.txt > 32BMP6meth.txt
awk '{print $2}' 33BMP6filt.txt > 33BMP6meth.txt
awk '{print $2}' 34BMP6filt.txt > 34BMP6meth.txt
awk '{print $2}' 35BMP6filt.txt > 35BMP6meth.txt
awk '{print $2}' 36BMP6filt.txt > 36BMP6meth.txt
awk '{print $2}' 37BMP6filt.txt > 37BMP6meth.txt
awk '{print $2}' 38BMP6filt.txt > 38BMP6meth.txt
awk '{print $2}' 39BMP6filt.txt > 39BMP6meth.txt
awk '{print $2}' 40BMP6filt.txt > 40BMP6meth.txt
awk '{print $2}' 41BMP6filt.txt > 41BMP6meth.txt
awk '{print $2}' 42BMP6filt.txt > 42BMP6meth.txt
awk '{print $2}' 43BMP6filt.txt > 43BMP6meth.txt
awk '{print $2}' 44BMP6filt.txt > 44BMP6meth.txt
awk '{print $2}' 45BMP6filt.txt > 45BMP6meth.txt
awk '{print $2}' 46BMP6filt.txt > 46BMP6meth.txt
awk '{print $2}' 47BMP6filt.txt > 47BMP6meth.txt


paste 01BMP6meth.txt 02BMP6meth.txt 03BMP6meth.txt 04BMP6meth.txt 05BMP6meth.txt 06BMP6meth.txt 07BMP6meth.txt 08BMP6meth.txt 09BMP6meth.txt 10BMP6meth.txt 11BMP6meth.txt 12BMP6meth.txt 13BMP6meth.txt 14BMP6meth.txt 15BMP6meth.txt 16BMP6meth.txt 17BMP6meth.txt 18BMP6meth.txt 19BMP6meth.txt 20BMP6meth.txt 21BMP6meth.txt 22BMP6meth.txt 23BMP6meth.txt 24BMP6meth.txt 25BMP6meth.txt 26BMP6meth.txt 27BMP6meth.txt 28BMP6meth.txt 33BMP6meth.txt 34BMP6meth.txt 35BMP6meth.txt 36BMP6meth.txt 37BMP6meth.txt 38BMP6meth.txt 39BMP6meth.txt 40BMP6meth.txt 41BMP6meth.txt 42BMP6meth.txt 43BMP6meth.txt 44BMP6meth.txt 45BMP6meth.txt 46BMP6meth.txt 47BMP6meth.txt > fullBMP6meth.txt

## sort methylation data  according to probe start site
sort -nk3 fullBMP6meth.txt > fullBMP6methsort.txt

## export text file into excel
cat fullBMP6methsort.txt fullBMP6methsort.xls

## to be worked on R studio
library(gplots)
library(colourbrewer)

## import text file into R 
##read in data
library(readxls)
BMP6 <- read_excel(“~/Desktop/TCGA-DLBCL/fullBMP6methsort.xlsx”)
View(BMP6)

##construct heatmap
BMP6data = data.matrix(‘BMP6’[4:50])             ##convert data into datamatrix
BPMPheatmap = heatmap.2(BMP6data,                ##dataframe
						main = "BMP6",     ##name of heat map
						trace = “none",     ##turns off trace lines in heat map
            margins = c(5,7),   ##define margin around plot
						dendrogram = "none",##turns off dendrogram							   		Rowv = NULL,        ##turns off row clustering
						Colv = NULL,        ##turns off column clustering
						key = TRUE          ##show colour key
							)

