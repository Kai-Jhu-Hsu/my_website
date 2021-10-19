---
categories:
- ""
- ""
date: "2021-10-18"
description: I am currently doing my master degree at LBS.
draft: false
image: download.png
keywords: ""
slug: aliquam
title: Project Example
---

# We analysed data about Airbnb listings and fit a model to predict the total cost. 

>Below is part of our codes as an example

>listings_resid_test <-listings_train %>% 
  filter(is.numeric(accommodates) == TRUE,is.numeric(availability_30) == TRUE, is.na(reviews_per_month) == FALSE, is.na(room_type) == FALSE, is.numeric(district_dummy) == TRUE,  is.numeric(instant_bookable_dummy) == TRUE) #%>% 

>plot1= ggplot(listings_resid_test,aes(accommodates , residuals(model_5))) + geom_point() + geom_smooth()
plot2=ggplot(listings_resid_test, aes(availability_30, residuals(model_5))) + geom_point() + geom_smooth()
plot3=ggplot(listings_resid_test, aes(reviews_per_month, residuals(model_5))) + geom_point() + geom_smooth()
plot4=ggplot(listings_resid_test, aes(review_scores_rating, residuals(model_5))) + geom_point() + geom_smooth()
plot5=ggplot(listings_resid_test, aes(room_type, residuals(model_5))) + geom_point() + geom_smooth()
plot6=ggplot(listings_resid_test, aes(district_dummy , residuals(model_5))) + geom_point() + geom_smooth()
plot7=ggplot(listings_resid_test, aes(instant_bookable_dummy, residuals(model_5))) + geom_point() + geom_smooth()
 / 

>grid.arrange(plot1,plot2,plot3,plot4,
             #plot5,plot6,plot7,#plot8,plot9,plot10,
             ncol=2,nrow=2)
             
             
  



