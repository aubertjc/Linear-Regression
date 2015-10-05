# Linear-Regression
Linear Regression
head(father.son)
ggplot(father.son,aes(x=fheight,y=sheight))+geom_point()+geom_smooth(method="lm")+labs(x="Fathers", y="Sons")
heightsLM<-lm(sheight~fheight, data=father.son)
heightsLM
summary(heightsLM)

ggplot(father.son,aes(x=fheight,y=sheight))+geom_point()+geom_smooth(method="lm")+labs(x="Fathers", y="Sons") + theme(panel.background = element_rect(fill = "navy"))

ggplot(father.son,aes(x=fheight,y=sheight))+geom_point()+geom_smooth(method="lm")+labs(x="Fathers", y="Sons") + theme(panel.background = element_rect(fill = "blue"))

ggplot(father.son,aes(x=fheight,y=sheight))+geom_point()+geom_smooth(method="lm")+labs(x="Fathers", y="Sons") + theme(panel.background = element_rect(fill = "light blue"))

ggplot(father.son,aes(x=fheight,y=sheight))+geom_point()+geom_smooth(method="lm")+labs(x="Fathers", y="Sons") + theme(panel.background = element_rect(fill = "orange"))

ggplot(father.son,aes(x=fheight,y=sheight))+geom_point()+geom_smooth(method="lm")+labs(x="Fathers", y="Sons") + theme(panel.background = element_rect(fill = "yellow"))

[mosaicplot(fheight ~ sheight, data = father.son, shade = TRUE, main = "Graphe en mosaïque")]

