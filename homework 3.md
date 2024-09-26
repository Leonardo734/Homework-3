# homework 3 
load("Household_Pulse_data_ph4c2.RData")
library(tidyverse)
library(ggplot2)
library(ggthemes)
library(dplyr)


#successful 
ggplot(Household_Pulse_data, aes(x = RECVDVACC, fill =factor(EGENID_BIRTH))) +
geom_bar() + labs(title = 'Gender and Vaccination Status', subtitle = 'BIRTH GENDER', y = 'Number of People', x = 'Vaccination Status') + theme_economist_white()




# This data only asks the birth gender of the recipents. They were also asked about their gender description however too many people answered NA so it is very difficult to analysis that data set. For the people who did get vaccined, a little over half of them(over 25000), were male and those who did not get vaccined, a little over half (over 5000) were female.As for the NA, it is looks to have slight majority of women. This means that men were overall men were more likely to get the vaccine.   