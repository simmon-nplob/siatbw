    일반 디스크 수명 점검 및 동작시간 확인용 프로그램으로 쉘로 작성하였습니다.
    한번에 장착된 다수의 디스크를 쉽게 점검하고 확인 할 수 있습니다
    해당 프로그램은 smartctl 프로그램을 활용하여 한번에 확인하고자 작성하였습니다.

    This is a written in Bashell program for disk check status - lifetime and operating time.
    You can easily check and confirm multiple disks mounted at once.
    This program was created so that it can be checked at once using the smartctl program.

    # chmod u+x runSIATBW
    # cp runSIATBW /usr/bin/
    # runSIATBW

    root@missA:/home/simmon/siatbw# ./runSIATBW 
    SCAN Your Disk INFO
    staus sata or sas
    sda: 238.47 GiB, 256060514304 bytes, 500118192 sectors
    sdb: 931.51 GiB, 1000204886016 bytes, 1953525168 sectors
    sdc: 931.51 GiB, 1000204886016 bytes, 1953525168 sectors
    sdd: 931.51 GiB, 1000204886016 bytes, 1953525168 sectors
    -------------------------------------------------------------------------
    status nvme
    -------------------------------------------------------------------------
                                                                         
    CHECK or SCAN Disk Name  sda sdb 
    OK, Enter your device name above: sda sdb sdc sdd
                                                                            
    TEST number of your Disk : 4
                                                                          
    Input Device Name:  sda 
    RAW Date Value - PROCESSING                        
    -------------------------------------------------------
    on_time: 1995  Power_Cycle_Count 509
    SDD Value - Wear_Leveling_Count: 9 POR_Recovery_Count: 82 lbs_written: 3968714882
    HDD Value - Spin_Up_Time:  Start_Stop_Count: 
    TBW-usage: 1892.43 GB [ 1.84808 TB ]
    TBW Device Name: SamsungSSD860PRO  sda test completed
    -------------------------------------------------------
    Input Device Name:  sdb 
    RAW Date Value - PROCESSING                        
    -------------------------------------------------------
    on_time: 342  Power_Cycle_Count 185
    SDD Value - Wear_Leveling_Count:  POR_Recovery_Count:  lbs_written: 
    HDD Value - Spin_Up_Time: 3783 Start_Stop_Count: 188
    TBW-usage:  GB [ 0 TB ]
    TBW Device Name: HGSTHUS722T1TALA604  sdb test completed
    -------------------------------------------------------
    Input Device Name:  sdc 
    RAW Date Value - PROCESSING                        
    -------------------------------------------------------
    on_time: 201  Power_Cycle_Count 70
    SDD Value - Wear_Leveling_Count:  POR_Recovery_Count:  lbs_written: 
    HDD Value - Spin_Up_Time: 3791 Start_Stop_Count: 74
    TBW-usage:  GB [ 0 TB ]
    TBW Device Name: HGSTHUS722T1TALA604  sdc test completed
    -------------------------------------------------------
    Input Device Name:  sdd 
    RAW Date Value - PROCESSING                        
    -------------------------------------------------------
    on_time: 184  Power_Cycle_Count 71
    SDD Value - Wear_Leveling_Count:  POR_Recovery_Count:  lbs_written: 
    HDD Value - Spin_Up_Time: 3800 Start_Stop_Count: 74
    TBW-usage:  GB [ 0 TB ]
    TBW Device Name: HGSTHUS722T1TALA604  sdd test completed
    -------------------------------------------------------
     S I A T B W Program Terminated! ------------------------  💗system by simmon 
