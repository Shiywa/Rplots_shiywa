# Rplots_shiywa
coding programe of beautiful R plots
# Boxplot
```
library(ggpubr)
my_comparisons <- list(c("HI-Mock","Mild"),c("HI-Mock","Moderate"),c("HI-Mock","Severe"))
p <- ggboxplot(xaf1, x = "group", y = "Value",
          color = "group", palette = "lancet",
          add = "jitter",short.panel.labs = FALSE,nrow = 1)+
  stat_compare_means(comparisons = my_comparisons,label = "p.format",method = "wilcox.test")+
  theme(axis.text.x = element_text(angle = 45,hjust = 1,vjust = 1))
p
```
![GSE135964_XAF1_exp](https://github.com/Shiywa/Rplots_shiywa/assets/42604587/3a637211-74e6-4ecd-b892-57ef8ff05b0f)

