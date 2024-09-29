# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Calculating Marginal Effects and Levels with Errors Using the Delta Method Use modmarg With (In) R Software
install.packages("modmarg")
library("modmarg")
modmarg = read.csv("https://raw.githubusercontent.com/timbulwidodostp/modmarg/main/modmarg/modmarg.csv",sep = ";")
# Estimation Calculating Marginal Effects and Levels with Errors Using the Delta Method Use modmarg With (In) R Software
modmarg <- glm(Sepal.Length ~ Sepal.Width + Species, data = modmarg, family = 'gaussian')     
# Predicted Levels
modmarg::marg(modmarg, var_interest = 'Species', type = 'levels')
# Predicted Effects
modmarg::marg(modmarg, var_interest = 'Species', type = 'effects')
# Calculating Marginal Effects and Levels with Errors Using the Delta Method Use modmarg With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished