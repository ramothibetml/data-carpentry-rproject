str(surveys)
#Select colums
select(surveys,species_id,weight)
#select rows
filter(surveys,year==1995)
#%>% pipes: %>% 
# use filter to select 
 surveys %>% 
   filter(year==1995) %>%
   select(species_id,weight) 
 #select only the rows with species weight less than 5, then select only species id,sex and weight
 
 exercise <- surveys %>% 
   filter(weight<5) %>%
   select(species_id,weight,sex)
#create new column
 #mutate
 data_with_kg <- surveys %>% 
   mutate(weight_kg=weight/1000)
 
 surveys %>% 
   mutate(weight_kg=weight/1000,weight_kg2=weight_kg*2)
 
   mutate(weight_kg=we
#remove the missing   o
 
#Using Head to selct the first rows
 surveys %>%
   filter(!is.na(weight)) %>% 
   mutate(weight_kg=weight/1000,weight_kg2=weight_kg*2) %>% 
   head()
 
 #Using the previous command
 #remove the missing values first (using filter), and re-run
 surveys %>%
   group_by(sex) %>% 
   summarise(mean_weight=mean(weight,na.rm = TRUE))

 #Group by two columns
 surveys %>%
   filter(!sex=="") %>% 
   group_by(sex) %>% 
   summarise(mean_weight=mean(weight,na.rm = TRUE))
   
 
 surveys %>%
   filter(!sex=="M"|sex=="F") %>% 
   group_by(sex) %>% 
   summarise(mean_weight=mean(weight,na.rm = TRUE))
 
 surveys %>%
   filter(!sex=="") %>% 
   filter(!is.na(weight)) %>% 
   group_by(sex,species_id) %>% 
   summarise(mean_weight=mean(weight,na.rm = TRUE))
 
 
 
 summarise_two <- surveys %>%
   filter(!sex=="") %>% 
   filter(!is.na(weight)) %>% 
   group_by(sex,species_id) %>% 
   summarise(mean_weight=mean(weight,na.rm = TRUE))
 # use the previous commands by add a new column that gives the minimum weight(and maximum weight)
 
 summarise_min_max <- surveys %>%
   filter(!sex=="") %>% 
   filter(!is.na(weight)) %>% 
   group_by(sex,species_id) %>% 
   summarise(mean_weight=mean(weight,na.rm = TRUE),min_weight=min(weight),max_weight=max(weight)
 #counting -filter means keep
 surveys %>% 
   filter(!sex=="") %>% 
   count(sex)
 #counting with two variables(how many sex and species)
 surveys %>% 
   filter(!sex=="") %>% 
   count(sex,species)
 
 #Sorting (arrange))
 surveys %>% 
   filter(!sex=="") %>% 
   count(sex,species) %>% 
 arrange(species,desc(n))

 
 
 #Reshaping   data
 
 
 
 
   