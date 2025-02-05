# Module4
Frequency <- c(0.6,0.3,0.4,0.4,0.2,0.6,0.3,0.4,0.9,0.2)
BP <- c(103,87,32,42,59,109,78,205,135,176)
First <- c(1,1,1,1,0,0,0,0,NA,1)
Second <- c(0,0,1,1,0,0,1,1,1,1)
FinalDecision <- c(0,1,0,1,0,1,0,1,1,1)

patients_data <- data.frame(Frequency, BP, First, Second, FinalDecision)

par(mfrow = c(1, 1))

boxplot(BP ~ First, data = patients_data,
        main = "BP vs First Doctor's Assessment",
        xlab = "First Doctor's Assessment (1 = bad, 0 = good)",
        ylab = "Blood Pressure")

boxplot(BP ~ Second, data = patients_data,
        main = "BP vs Second Doctor's Assessment",
        xlab = "Second Doctor's Assessment (1 = high, 0 = low)",
        ylab = "Blood Pressure")

hist(patients_data$BP,
     main = "Histogram of Blood Pressure",
     xlab = "Blood Pressure",
     ylab = "Frequency",
     col = "blue")
     ![image](https://github.com/user-attachments/assets/5f8fd006-33ec-46f7-a019-aba5885f1ec6)
     ![image](https://github.com/user-attachments/assets/22471adc-60c6-49e1-a103-7fe7b6a1c499)
     ![image](https://github.com/user-attachments/assets/78731c75-27a8-4a5a-a171-47b70b8be1db)
    
     
     


