# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Transformation-free Linear Regression for Compositional Outcomes and Predictors Use codalm With (In) R Software
install.packages("codalm")
library("codalm")
codalm = read.csv("https://raw.githubusercontent.com/timbulwidodostp/codalm/main/codalm/codalm.csv",sep = ";")
# Estimation Transformation-free Linear Regression for Compositional Outcomes and Predictors Use codalm With (In) R Software
father <- as.matrix(codalm[,3:5])
y <- father / rowSums(father)
mother <- as.matrix(codalm[,6:8])
x <- mother/rowSums(mother)
codalm <- codalm(y, x)
codalm
# Transformation-free Linear Regression for Compositional Outcomes and Predictors Use codalm With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished