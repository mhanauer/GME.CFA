# GME.CFA
data = read.csv("GME.csv", header = TRUE)
names(data)
data = data[c(135,136,137,138,139,140)]
data = na.omit(data)
data
data.sd = apply(data,2,sd)
data.sd
write.csv(data, "GMEData.csv")
