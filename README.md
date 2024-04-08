    일반 디스크 수명 점검 및 동작시간 확인용 프로그램으로 쉘로 작성하였습니다.
    한번에 장착된 다수의 디스크를 쉽게 점검하고 확인 할 수 있습니다
    해당 프로그램은 smartctl 프로그램을 활용하여 한번에 확인하고자 작성하였습니다.

    시험된 OS: Rehel9.3 계열/Rocky9.3, Centos7, Fedora 40/39 Server, Ubuntu 22.04LTS

    This is a written in Bashell program for disk check status - lifetime and operating time.
    You can easily check and confirm multiple disks mounted at once.
    This program was created so that it can be checked at once using the smartctl program.

    # chmod u+x runSIATBW
    # cp runSIATBW /usr/bin/
    # runSIATBW

    root@missA:/home/simmon/siatbw# ./runSIATBW 
    SCAN Your Disk INFO
    status nvme
    -------------------------------------------------------------------------
    -------------------------------------------------------------------------
    staus sata or sas
    sda: 238.47 GiB, 256060514304 bytes, 500118192 sectors
    sdb: 931.51 GiB, 1000204886016 bytes, 1953525168 sectors
    sdc: 931.51 GiB, 1000204886016 bytes, 1953525168 sectors
    sdd: 931.51 GiB, 1000204886016 bytes, 1953525168 sectors
    -------------------------------------------------------------------------
                                                                        
    CHECK or SCAN Disk Name  sda sdb sdc 
    OK, Enter your device name above: sda sdb sdc sdd
    Show - input Disk: sda                                                                         
    TEST number of your Disk : 4
                                                                             
    -------------------------------------------------------------------------
    -------------------------------------------------------------------------
    Input Device Name:  sda 
    RAW Date Value - PROCESSING                       
    On_Time:   2001  Power_Cycle_Count:   510 
    NVME Disk - DATA Units Written:    DATA Units Read:   
    SDD  Disk - Wear_Leveling_Count:  9  POR_Recovery_Count:  82  lbs_written: 3975518361 
    HDD  Disk - Spin_Up_Time:    Start_Stop_Count:   
    TBW-usage: 1895.67 GB [ 1.85124 TB ] 
     ERROR Indicator Value -> RAW_Read_Error_Rate:    Reallocated_Sector_Ct: 0  Seek_Error_Rate:  
     Spin_Retry_Count:    Current_Pending_Sector:   Offline_Uncorrectable:    UDMA_CRC_Error_Count:  
    TBW Device Name:   SamsungSSD860PRO  sda test completed
    -------------------------------------------------------------------------
    -------------------------------------------------------------------------
    Input Device Name:  sdb 
    RAW Date Value - PROCESSING                       
    On_Time:   347  Power_Cycle_Count:   186 
    NVME Disk - DATA Units Written:    DATA Units Read:   
    SDD  Disk - Wear_Leveling_Count:    POR_Recovery_Count:    lbs_written:  
    HDD  Disk - Spin_Up_Time:  3775  Start_Stop_Count:  189 
    TBW-usage:  GB [ 0 TB ] 
     ERROR Indicator Value -> RAW_Read_Error_Rate:  0  Reallocated_Sector_Ct: 0  Seek_Error_Rate:  0
     Spin_Retry_Count:  0  Current_Pending_Sector: 0  Offline_Uncorrectable:  0  UDMA_CRC_Error_Count:  0
    TBW Device Name:   HGSTHUS722T1TALA604  sdb test completed
    -------------------------------------------------------------------------
    -------------------------------------------------------------------------
    Input Device Name:  sdc 
    RAW Date Value - PROCESSING                       
    On_Time:   206  Power_Cycle_Count:   71 
    NVME Disk - DATA Units Written:    DATA Units Read:   
    SDD  Disk - Wear_Leveling_Count:    POR_Recovery_Count:    lbs_written:  
    HDD  Disk - Spin_Up_Time:  3791  Start_Stop_Count:  75 
    TBW-usage:  GB [ 0 TB ] 
     ERROR Indicator Value -> RAW_Read_Error_Rate:  0  Reallocated_Sector_Ct: 0  Seek_Error_Rate:  0
     Spin_Retry_Count:  0  Current_Pending_Sector: 0  Offline_Uncorrectable:  0  UDMA_CRC_Error_Count:  0
    TBW Device Name:   HGSTHUS722T1TALA604  sdc test completed
    -------------------------------------------------------------------------
    -------------------------------------------------------------------------
    Input Device Name:  sdd 
    RAW Date Value - PROCESSING                       
    On_Time:   189  Power_Cycle_Count:   72 
    NVME Disk - DATA Units Written:    DATA Units Read:   
    SDD  Disk - Wear_Leveling_Count:    POR_Recovery_Count:    lbs_written:  
    HDD  Disk - Spin_Up_Time:  3800  Start_Stop_Count:  75 
    TBW-usage:  GB [ 0 TB ] 
     ERROR Indicator Value -> RAW_Read_Error_Rate:  0  Reallocated_Sector_Ct: 0  Seek_Error_Rate:  0
     Spin_Retry_Count:  0  Current_Pending_Sector: 0  Offline_Uncorrectable:  0  UDMA_CRC_Error_Count:  0
    TBW Device Name:   HGSTHUS722T1TALA604  sdd test completed
    -------------------------------------------------------------------------
     S I A T B W Program Terminated! ------------------------  💗system by simmon
