# Linux Commands, Tricks, Tips, etc.

# Display disk space 

df -H

du


# change filename 
#! /bin/bash  
for i in *_tumor_*.pkl; do mv $i ${i/*_tumor_/tumor_}; done

# bash command on HPC
[liw17@biowulf ~]$ history

    1  12:54  cd Figure5/
    
    2  12:54  ls .
    
    3  12:54  vi distofall.R
    
    4  14:24  sjobs
    
   10  20:37  sinfo
   
   11  12:15  module load emacs
   
   12  12:15  emacs
   
   13  12:17  emacs &
   
   14  12:17  detach %+ #
   
   16  11:56  module spider git
   
   18  17:35  sinteractive
   
   19  17:53  logout
   
   21  17:57  exit
   
   23  17:33  module spider emacs
   
   24  17:33  module load emacs/24.5
   
   25  17:33  emacs
   
   26  17:56  module spider genome
   
   27  17:57  module load pseudogenome/2015-04-01
   
   28  17:58  exit
   
   29  17:13  sinteractive
   
   30  17:53  sinteractive
   
   31  17:58  logout
   
   32  17:32  sinteractive
   
   33  17:58  logout
   
   34  15:27  ls .
   
   35  15:27  cd Documents/
   
   36  15:27  cd Figure5/
   
   37  15:27  ls .
   
   38  15:27  vi F5CD4PCF.R
   
   39  15:37  ls .
   
   40  15:37  ls -al
   
   41  15:37  vi F5CD4PCF.R
   
   42  15:41  ls .
   
   43  15:41  chmod 777 CD4K3EST.R
   
   44  15:41  chmod 777 F5CD4K3est.R
   
   45  15:42  ls .
   
   46  15:42  cd ..
   
   47  15:42  ls .
   
   48  15:42  vi F5CD4PCF.sh
   
   49  15:44  ls .
   
   50  15:45  mv CD4K3EST.sh F5CD4K3EST.sh
   
   51  15:45  ls .
   
   52  15:45  chmod 777 F5CD4K3EST.sh
   
   53  15:45  ls .
   
   54  15:49  sbatch --ntasks=64 --ntasks-per-core=1 [--mem-per-cpu=50g] F5CD4K3EST.sh
   
   55  15:50  sbatch --ntasks=64 --ntasks-per-core=1 --mem-per-cpu=50g F5CD4K3EST.sh
   
   56  15:50  sbatch --ntasks=24 --ntasks-per-core=1 --mem-per-cpu=20g F5CD4K3EST.sh
   
   57  15:51  sbatch --ntasks=5 --ntasks-per-core=1 --mem-per-cpu=20g F5CD4K3EST.sh
   
   58  15:55  sjobs
   
   59  15:57  sbatch --ntasks=100 --ntasks-per-core=1 --mem-per-cpu=5g F5CD4K3EST.sh
   
   60  16:01  module spider parallel
   
   61  16:52  sjobs
   
   62  16:52  cd  Figure5/
   
   63  16:52  ls .
   64  16:53  cd ..
   65  16:53  ls .
   66  16:54  vi slurm_66857333.out
   
   67  16:55  vi cd  Figure5/
   68  16:55  cd Figure5/
   69  16:55  ls .
   70  16:55  vi F5CD4K3est.R
   71  17:05  sbatch --ntasks=50 --ntasks-per-core=1 --mem-per-cpu=10g F5CD4K3EST.sh
   72  17:06  cd ..
   73  17:06  sbatch --ntasks=50 --ntasks-per-core=1 --mem-per-cpu=10g F5CD4K3EST.sh
   74  17:06  sbatch -j=5  --ntasks-per-core=1 --mem-per-cpu=10g F5CD4K3EST.sh
   75  17:07  sbatch --ntasks=30 --ntasks-per-core=1 --mem-per-cpu=10g F5CD4K3EST.sh
   76  17:07  sbatch --ntasks=12 --ntasks-per-core=1 --mem-per-cpu=10g F5CD4K3EST.sh
   77  17:08  sjobs
   78  17:14  sjobs
   79  17:15  ls .
   80  17:15  vi slurm_66868711.out
   81  17:18  cd  Figure5/
   82  17:18  ls .
   83  17:18  vi CD4K3EST.R
   84  17:21  cd ..
   85  17:21  vi F5CD4K3EST.sh
   86  17:28  vi F3B220.sh
   87  17:28  cd Figure5/
   88  17:28  ls ,
   89  17:28  ls .
   90  17:29  vi F5B220PCF.R
   91  17:30  vi CD4K3EST.R
   92  17:33  sbatch --nodes=5 --ntasks-per-core=1 --mem-per-cpu=10g F5CD4K3EST.sh
   93  17:33  cd ..
   94  17:33  sbatch --nodes=5 --ntasks-per-core=1 --mem-per-cpu=10g F5CD4K3EST.sh
   95  17:36  sbatch --nodes=2  --mem=50g --cpus-per-task=50  F5CD4K3EST.sh
   96  14:33  module spider mpi
   97  15:03  sinteractive --constraint=multinode --ntasks=64 --exclusive
   98  15:04  sinteractive  --constraint=multinode  --ntasks=64  --exclusive
   99  15:04  sinteractive  --constraint=multinode  --ntasks=64
  100  15:06  sinteractive --mem=80g --cpus-per-task=50
  101  20:44  sinteractive
  102  17:21  module load
  103  17:21  module spider emacs
  104  17:21  module load emacs/24.5 .5
  105  17:21  module load emacs/24.5
  106  17:22  emacs
  107  17:23  sinteractive --mem=80g --cpus-per-task=100
  108  17:23  sinteractive --mem=80g --cpus-per-task=80
  109  17:23  sinteractive --mem=80g --cpus-per-task=50
  110  17:19  ls .
  111  17:20  emacs
  112  17:20  vi
  113  12:48  emacs
  114  13:01  logout
  115  13:01  exit
  116  18:28  ls .
  117  18:28  cd  Documents/
  118  18:28  ls .
  119  18:28  cd Figure5/
  120  18:28  ls .
  121  18:29  emacs F5B220PCF.R
  122  19:18  cd ..
  123  19:18  ls .
  124  19:21  emacs F5B220PCF.sh
  125  19:23  sbatch F5B220PCF.sh
  126  19:38  sjob0;40;41M0;40;41m0;42;40M0;42;40m
  127  19:38  sjobs
  128  19:39  ls . -al
  129  19:39  ls .
  130  19:40  emacs F5B220PCF.sh
  131  19:41  cd Figure5/
  132  19:41  ls .
  133  19:44  sinteractive
  134  22:01  sjobs
  135  11:27  ls .
  136  11:30  ls .
  137  12:47  ls .
  138  12:47  emacs
  139  12:48  sinteractive
  140  11:55  exit
  141  12:55  module spider matlab
  142  12:55  module load matlab/2018a
  143  12:55  matlab
  144  12:58  module load matlab/2017b
  145  12:59  matlab
  146  14:17  module spider matlab
  147  14:17  module load matlab/2013a
  148  14:17  matlab
  149  17:43  module load matlab/2012b
  150  17:43  matlab
  151  11:26  ls .
  152  11:26  matlab
  153  11:28  exit
  154  11:44  module load emacs/24.5
  155  11:44  emacs
  156  11:47  exit
  157  17:39  module spider matlab
  158  17:39  module load matlab/2012b
  159  17:40  sinteractive --mem=80g --cpu-per-task=50 --time=20:00:00
  160  17:41  sinteractive --mem=80g --cpus-per-task=50 --time=20:00:00
  161  17:46  sinteractive --mem=80g --cpus-per-task=50 --time=02:00:00
  162  17:53  sinteractive --mem=80g --cpus-per-task=50
  163  19:46  module spider matlab
  164  19:48  module load matlab/2018a
  165  19:59  sinteractive --mem=80g --cpus-per-task=50 --time=12:00:00
  166  22:16  sinteractive --mem=80g --cpus-per-task=50 --time=12:00:00
  167  07:17  sinteractive --mem=80g --cpus-per-task=50 --time=12:00:00
  168  11:48  module spider emacs
  169  11:48  module load emacs/24.5
  170  11:48  emacs
  171  12:55  sinteractive --mem=80g --cpus-per-task=50 --time=24:00:00
  172  11:28  sinteractive --mem=80g --cpus-per-task=50 --time=48:00:00
  173  12:03  sinteractive --mem=80g --cpus-per-task=50 --time=24:00:00
  174  09:57  ls .
  175  09:57  cd Documents/
  176  09:57  ls .
  177  09:58  cd Figure5/
  178  09:58  ls .
  179  09:58  vi F5CD4K3est.R
  180  10:03  vi F5CD4PCF.R
  181  10:10  ls -al
  182  10:10  chmod 777 F5CD4PCF.R
  183  10:10  ls -al
  184  10:10  cd ..
  185  10:10  ls .
  186  10:11  vi F5CD4PCF.sh
  187  10:14  sbatch --mem=80g --cpus-per-task=50 --time=2:00:00 F5CD4PCF.sh
  188  10:14  cd Figure5/
  189  10:14  ls .
  190  10:16  vi F5CD8PCF.R
  191  10:17  vi F5CD4PCF.R
  192  10:18  vi F5CD8PCF.R
  193  10:23  cd ..
  194  10:23  vi F5CD8PCF.sh
  195  10:24  sbatch --mem=80g --cpus-per-task=50 --time=2:00:00 F5CD8PCF.sh
  196  10:24  sjobs
  197  10:25  cd Figure5/
  198  10:25  ls .
  199  10:25  vi F5B220PCF.R
  200  10:29  ls .
  201  10:30  cd ..
  202  10:30  ls .
  203  10:30  vi F5B220PCF.sh
  204  10:31  sbatch F5B220K3.sh
  205  10:31  sjobs
  206  10:33  cd Figure5/
  207  10:33  ls -al
  208  10:33  cd ..
  209  10:33  ls -al
  210  10:34  vi slurm_308293.out
  211  10:34  cd Figure5/
  212  10:34  ls .
  213  10:35  vi F5CD4PCF.R
  214  10:36  sbatch --mem=80g --cpus-per-task=50 --time=2:00:00 F5CD4PCF.sh
  215  10:36  cd ..
  216  10:36  sbatch --mem=80g --cpus-per-task=50 --time=2:00:00 F5CD4PCF.sh
  217  10:36  sjobs
  218  10:37  cd Figure5/
  219  10:37  ls .
  220  10:37  vi F5CD8PCF.R
  221  10:37  sjobs
  222  10:38  sbatch --mem=80g --cpus-per-task=50 --time=2:00:00 F5CD8PCF.sh
  223  10:38  cd ..
  224  10:38  sbatch --mem=80g --cpus-per-task=50 --time=2:00:00 F5CD8PCF.sh
  225  10:41  sjobs
  226  11:11  sjobs
  227  11:21  sjobs
  228  11:31  sjobs
  229  11:42  cd Documents/
  230  11:42  ls .
  231  11:42  cd Figure5/
  232  11:42  ls .
  233  11:42  vi F5CD8PCF.R
  234  11:46  sbatch --mem=80g --cpus-per-task=50  --time=2:00:00 F5CD8PCF.sh
  235  11:46  cd ..
  236  11:46  ls .
  237  11:46  ls -al
  238  11:47  sbatch --mem=80g --cpus-per-task=50  --time=2:00:00 F5CD8PCF.sh
  239  11:47  cd Figure5/
  240  11:47  ls .
  241  11:48  vi F5CD8PCF.R
  242  12:07  cd Documents/
  243  12:07  cd Figure5/
  244  12:07  ls .
  245  12:07  vi F5CD8PCF.R
  246  12:08  ls -al
  247  12:08  sjobs
  248  12:09  cd ..
  249  12:09  ls .
  250  12:09  vi F5CD8PCF.sh
  251  12:10  sbatch --mem=80g --cpus-per-task=50 --time=1:00:00 F5CD8PCF.sh
  252  12:10  sjobs
  253  12:11  sjobs
  254  12:11  sbatch --mem=80g --cpus-per-task=50 --time=30:00 F5CD8PCF.sh
  255  12:11  cd Figure5/
  256  12:11  ls .
  257  12:12  vi F5CD8PCF.R
  258  12:13  cd ..
  259  12:13  sjobs
  260  12:43  sjobs
  261  12:43  cd Documents/
  262  12:43  cd  Figure5/
  263  12:43  ls .
  264  12:44  vi F5CD8PCF.R
  265  12:44  ls -al
  266  13:04  sjobs
  267  13:04  ls
  268  15:12  ls .
  269  15:12  cd Documents/
  270  15:12  ls .
  271  15:13  cd Figure5/
  272  15:13  ls .
  273  16:12  ls .
  274  16:13  clear
  275  16:17  cd  Documents/
  276  16:17  ls .
  277  16:19  cd Figure5/
  278  16:19  ls .
  279  16:20  vi F5CD4PCF.R
  280  16:41  ls .
  281  16:41  cd ..
  282  16:41  ls .
  283  16:41  vi F5CD4PCF.sh
  284  16:42  ls .
  285  16:44  sbatch --mem=80g --cpus-per-task=50 F5CD4CD8PCFK.sh
  286  16:45  cd Figure5/
  287  16:45  ls .
  288  16:45  vi F5CD4PCF.R
  289  17:06  cd ..
  290  17:06  ls .
  291  17:07  vi F5CD4CD8PCFK.sh
  292  17:07  cd Figure5/
  293  17:07  ls.
  294  17:07  ls .
  295  17:07  sjobs
  296  17:08  vi F5CD4CD8PCFK.R
  297  17:09  vi F5CD4CD8PCFK.R
  298  17:13  cd ..
  299  17:15  vi F5CD4CD8PCFK.sh
  300  17:16  ls .
  301  17:16  cd Figure5/
  302  17:16  ls .
  303  17:17  cd ..
  304  17:17  vi F5CD4CD8PCFKFULL.sh
  305  17:19  sbatch --mem=80g --cpus-per-task=50  F5CD4CD8PCFKF.sh
  306  17:19  sbatch --mem=80g --cpus-per-task=50  F5CD4CD8PCFKFULL.sh
  307  17:21  cd Figure5/
  308  17:21  ls .
  309  17:22  vi F5CD4CD8PCFK.R
  310  17:23  vi F5CD4CD8PCFKF.R
  311  17:28  sjobs
  312  17:31  cd ..
  313  17:31  cd ..
  314  17:43  cd Documents/Figure5/
  315  17:44  ls .
  316  18:03  sjobs
  317  18:15  sjobs
  318  18:16  vi F5CD4CD8PCFK.R
  319  17:05  vi F5CD4PCF.R F5CD4CD8PCFK.R
  320  19:05  cd Documents/
  321  19:05  cd Figure5/
  322  19:05  ls .
  323  19:08  vi F5CD4PCF.R
  324  19:34  sjobs
  325  20:14  vi F5CD4PCF.R
  326  22:08  sinteractive --mem=200g --cpus-per-task=50 --time=20:00:00
  327  22:17  sinteractive --mem=100g --cpus-per-task=50 --time=20:00:00
  328  21:02  ls .
  329  21:02  cd Documents/
  330  21:02  ls .
  331  21:02  cd Figure5/
  332  21:02  ls .
  333  21:02  vi F5B220PCF.R
  334  21:04  ls .
  335  21:05  cd ..
  336  21:05  ls .
  337  21:05  vi F5B220PCF.sh
  338  21:06  cd Figure5/
  339  21:06  ls .
  340  21:06  cd ..
  341  21:06  vi F5B220PCF.sh
  342  21:10  sbatch --mem=80g --cpus-per-task=50 F5B220PCF.sh
  343  21:20  sjobs
  344  21:21  sjobs
  345  22:01  sjobs
  346  22:02  cd Figure5/
  347  22:02  ls .
  348  22:02  vi F5B220PCF.R
  349  22:12  cd ..
  350  22:12  sjobs
  351  15:04  module load singularity
  352  15:04  sigularity
  353  15:04  singularity
  354  15:07  singularity  shell TF.image.simg
  355  15:14  exit
  356  15:14  module load singularity
  357  15:15  singularity  shell TF.image.simg
  358  15:16  exit
  359  21:26  ls .
  360  21:33  sinteractive --gres=gpu:k20x:1 --nv
  361  21:35  history
  362  21:37  sinteractive --partition=gpu -nv  --gres=gpu:p100
  363  21:37  sinteractive  -nv  --gres=gpu:p100
  364  21:37  sinteractive  --nv  --gres=gpu:p100
  365  21:41  sinteractive --constraint=gpuk80 --gres=gpu:k80:1
  366  14:52  ls .
  367  14:53  ls -al
  368  15:03  sinteractive --cpus-per-task=4 --mem=10g
  369  15:14  sinteractive --gres=gpu:k20x:1
  370  15:16  sinteractive --gres=gpu:p100:1
  371  18:42  sinteractive --gres=gpu:p100:1
  372  18:44  freen
  373  18:44  sinteractive --gres=gpu:p100:1 -c 10
  374  09:16  sinteractive --gres=gpu:p100:1 -c 10
  375  09:16  exit
  376  09:17  logout
  377  12:26  sinteractive --gres=gpu:p100:1
  378  11:01  module load singularity
  379  11:02  sudo singularity shell TF.image.simg
  380  11:02  sudo singularity shell TF.image.simg
  381  11:04  sudo singularity shell TF.image.simg
  382  11:05  sudo singularity shell TF.image.simg
  383  11:07  singularity shell TF.image.simg
  384  11:20  singularity shell kerasWithMASKRCNN-0.simg
  385  11:21  singularity shell --nv kerasWithMASKRCNN-0.simg
  386  11:23  checkquota
  387  11:23  sjobs
  388  11:25  exit
  389  21:59  ls .
  390  21:59  freen
  391  22:02  sinteractive --gres=gpu:p100:1 --cpus-per-task=20 --time = 8:00:00
  392  22:02  sinteractive --gres=gpu:p100:1 --cpus-per-task=20 --time = 10:00:00
  393  22:03  sinteractive --gres=gpu:p100:1 --cpus-per-task=20 --time = 2-00:00:00
  394  22:04  sinteractive --gres=gpu:p100:1 --cpus-per-task=20 --time = 10:00:00
  395  22:10  sinteractive --gres=gpu:p100:1 --cpus-per-task=20 -time = 10:00:00
  396  22:11  sinteractive --gres=gpu:p100:1 --cpus-per-task=20
  397  22:14  sinteractive --gres=gpu:p100:1 --cpus-per-task=8
  398  10:54  sinteractive --gres=gpu:k20x:1 --cpus-per-task=8
  399  11:01  sinteractive --gres=gpu:k20x:1
  400  11:25  sinteractive --gres=gpu:p100:1
  401  11:28  ls -al
  402  11:29  chmod 777 kerasWithMASKRCNN-0.simg
  403  11:29  ls -al
  404  11:29  sinteractive --gres=gpu:k80x:1
  405  11:29  freen
  406  11:29  sinteractive --gres=gpu:k80:1
  407  11:30  sinteractive --gres=gpu:p100:1
  408  11:35  freen
  409  11:35  sinteractive --gres=gpu:k80:1
  410  11:06  ls .
  411  11:06  cd  Documents/
  412  11:06  ls .
  413  11:07  cd ..
  414  11:07  ls .
  415  11:07  rm TF.image.simg
  416  11:07  ls .
  417  11:07  cd Documents/
  418  11:07  ls .
  419  11:07  rm newTF.simg
  420  11:07  ls .
  421  11:37  module load singularity
  422  11:37  singularity shell --nv Documents/newlease.simg
  423  11:49  singularity shell --nv Documents/newlease.simg
  424  11:50  exit
  425  11:36  sinteractive --gres=gpu:p100:1
  426  11:50  freen
  427  11:52  sinteractive --gres=gpu:p100:1 --cpus-per-task=8
  428  21:58  checkquota
  429  21:59  ls .
  430  21:59  cd Downloads/
  431  21:59  ls .
  432  21:59  rm Amira-620-Linux64-gcc44-Debug.tar.bz2
  433  21:59  ls -al
  434  22:00  checkquota
  435  22:01  rm Amira-620-Linux64-gcc44.bin
  436  22:01  ls -al
  437  22:01  checkquota
  438  22:02  cd ..
  439  22:02  cd Documents/
  440  22:02  ls .
  441  22:02  ls  -al
  442  22:02  rm kerastensornew.img
  443  22:36  ls .
  444  22:36  rm kerasWithMASKRCNN-0.simg
  445  22:53  fr
  446  22:53  freen
  447  22:55  sinteractive --gres=gpu:p100:1 --cpus-per-task=8
  448  09:36  sinteractive --gres=gpu:p100:1 --cpus-per-task=8
  449  22:25  freen
  450  22:26  sinteractive --gres=gpu:k80:1 --cpus-per-task=8
  451  06:37  freen
  452  06:37  sinteractive --gres=gpu:p100:1 --cpus-per-task=8
  453  20:19  ls
  454  20:19  cd Documents/
  455  20:19  ls .
  456  20:19  rm kerastensorbestmatch.simg
  457  20:19  rm kerastensornewnew.img
  458  20:36  ls .
  459  20:36  freen
  460  20:37  sinteractive --gres=gpu:p100:1 --cpus-per-task=8
  461  07:04  cd Documents/
  462  07:06  vi 0918googlenetpred.py
  463  07:38  cd /data
  464  07:38  cd liw17
  465  07:38  ls .
  466  07:38  cd CAMELYON16/
  467  07:39  ls
  468  07:39  cd training/
  469  07:39  ls .
  470  07:39  cd tumor/
  471  07:39  ls .
  472  07:39  ls -al
  473  07:40  cp tumor_036.tif ~/Documents/
  474  07:41  cd ~/Documents/
  475  07:41  vi 0918googlenetpred.py
  476  07:41  vi 0918googlenetpred.py
  477  06:55  module load singularity
  478  06:55  sinteractive --gres=gpu:p100:1
  479  08:49  nvidia-smi
  480  08:45  ls .
  481  08:45  cd Documents/
  482  08:45  ls .
  483  08:45  sinteractive --gres=gpu:p100:1
  484  16:07  cd Documents/
  485  16:07  module load singularity
  486  16:07  singularity shell -nv TFkeras0925.simg
  487  16:07  singularity shell --nv TFkeras0925.simg
  488  17:21  nvidia-smi
  489  17:21  exit
  490  16:02  cd Documents/
  491  16:02  ls .
  492  16:03  rm TFkeras0924.simg
  493  16:31  vi 0918googlenetpred.py
  494  16:39  vi 0918googlenetpred.py
  495  16:43  nvidia-smi
  496  16:45  vi 0918googlenetpred.py
  497  17:19  ls .
  498  14:58  ls ~/Documents/eICUCollaborativeadmissionDrug.csv
  499  16:01  exit
  500  18:08  ls .
  501  10:27  ls .
  502  10:27  ls Downloads/
  503  10:27  ls  Documents/
  504  10:28  freenode
  505  10:28  freen
  506  10:30  history
