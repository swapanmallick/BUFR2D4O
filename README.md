# BUFR2D4O
# STEP-1: 
   Copy /work/csp/sm09722/b2d4o/D4O_PREPROCESS.job 
    D4O_PREPROCESS.job is the main script to submit a job

# STEP-2:
    > bsub <  D4O_PREPROCESS.job
 If everything is good and Zeus works appropriately. It will create a folder inside the same directory.

 YYYY/MM/YYYYMMDDHR/*
   And you can see all the files inside the same folder, TS* all.
    

  Done!
  You are ready to use the files.

# STEP-3:

Now how to change date, input, output, and thinning, 

 1.  Open  D4O_PREPROCESS.job              
 2.  EVENT=201904.        Change the date                   
 3.  INPUTDIR=/data/csp/ss35621/BIG-DATA     For input data
 4.  thinning=16. Change here for thinning 4 or 16 as per requirement
 5.  source /data/csp/${USER}/d4o/install/INTEL/source.me 
 6.  Note binary files are available in /data/csp/sm09722/d4o/install/INTEL/d4o/bin
 7.  box2csv   bulk_create  catalogd4o          csv2sqlite  d4ojoin     d4omerge  d4osplit     mode_paste    obseqd4o  reduce_obs_count.pl  trim_pathbufr2d4o  calltree.pl  create_bufr_counts  d4odiff     d4ojoinall  d4oshow   gregdate.pl  nytprof-perl  odcsql    traceback_filter



  # Done!
  # You are ready to use the files.
