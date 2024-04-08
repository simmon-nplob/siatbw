    일반 디스크 수명 점검 및 동작시간 확인용 프로그램으로 쉘로 작성하였습니다.
    한번에 장착된 다수의 디스크를 쉽게 점검하고 확인 할 수 있습니다
    해당 프로그램은 smartctl 프로그램을 활용하여 한번에 확인하고자 작성하였습니다.

    시험된 OS: Rehel9.3 계열/Rocky9.3, Fedora 40 Server

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
    nvme0n1: 119.24 GiB, 128035676160 bytes, 250069680 sectors
    -------------------------------------------------------------------------
    staus sata or sas
    sdb: 931.51 GiB, 1000204886016 bytes, 1953525168 sectors
    sda: 931.51 GiB, 1000204886016 bytes, 1953525168 sectors
    sdc: 931.51 GiB, 1000204886016 bytes, 1953525168 sectors
    sdd: 931.51 GiB, 1000204886016 bytes, 1953525168 sectors
    -------------------------------------------------------------------------
                                                                    
    CHECK or SCAN Disk Name  sda sdb sdc 
    OK, Enter your device name above: nvme0n1 sda sdb sdc sdd
    Show - input Disk: nvme0n1                                                                         
    TEST number of your Disk : 5
                                                                         
    -------------------------------------------------------------------------
    -------------------------------------------------------------------------
    Input Device Name:  nvme0n1 
    RAW Date Value - PROCESSING                       
    On_Time:  4   Power_Cycle_Count:  64  
    NVME Disk - DATA Units Written:  [287GB]  DATA Units Read:  [312GB] 
    SDD  Disk - Wear_Leveling_Count:    POR_Recovery_Count:    lbs_written:  
    HDD  Disk - Spin_Up_Time:    Start_Stop_Count:   
    TBW-usage:  GB [ 0 TB ] 
    TBW Device Name:  SAMSUNGMZVLQ128HCHQ-00B   nvme0n1 test completed
    -------------------------------------------------------------------------
    -------------------------------------------------------------------------
    Input Device Name:  sda 
    RAW Date Value - PROCESSING                       
    On_Time:   2145  Power_Cycle_Count:   188 
    NVME Disk - DATA Units Written:    DATA Units Read:   
    SDD  Disk - Wear_Leveling_Count:    POR_Recovery_Count:    lbs_written:  
    HDD  Disk - Spin_Up_Time:  3825  Start_Stop_Count:  188 
    TBW-usage:  GB [ 0 TB ] 
    TBW Device Name:   HGSTHUS722T1TALA604  sda test completed
    -------------------------------------------------------------------------
    -------------------------------------------------------------------------
    Input Device Name:  sdb 
    RAW Date Value - PROCESSING                       
    On_Time:   2145  Power_Cycle_Count:   174 
    NVME Disk - DATA Units Written:    DATA Units Read:   
    SDD  Disk - Wear_Leveling_Count:    POR_Recovery_Count:    lbs_written:  
    HDD  Disk - Spin_Up_Time:  3833  Start_Stop_Count:  174 
    TBW-usage:  GB [ 0 TB ] 
    TBW Device Name:   HGSTHUS722T1TALA604  sdb test completed
    -------------------------------------------------------------------------
    -------------------------------------------------------------------------
    Input Device Name:  sdc 
    RAW Date Value - PROCESSING                       
    On_Time:   2155  Power_Cycle_Count:   196 
    NVME Disk - DATA Units Written:    DATA Units Read:   
    SDD  Disk - Wear_Leveling_Count:    POR_Recovery_Count:    lbs_written:  
    HDD  Disk - Spin_Up_Time:  3900  Start_Stop_Count:  196 
    TBW-usage:  GB [ 0 TB ] 
    TBW Device Name:   HGSTHUS722T1TALA604  sdc test completed
    -------------------------------------------------------------------------
    -------------------------------------------------------------------------
    Input Device Name:  sdd 
    RAW Date Value - PROCESSING                       
    On_Time:   2146  Power_Cycle_Count:   178 
    NVME Disk - DATA Units Written:    DATA Units Read:   
    SDD  Disk - Wear_Leveling_Count:    POR_Recovery_Count:    lbs_written:  
    HDD  Disk - Spin_Up_Time:  3833  Start_Stop_Count:  178 
    TBW-usage:  GB [ 0 TB ] 
    TBW Device Name:   HGSTHUS722T1TALA604  sdd test completed
    -------------------------------------------------------------------------
     S I A T B W Program Terminated! ------------------------  💗system by simmon 
     
