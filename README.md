1) Running the Code "simu_or_lcfdrn_scth.py": These instructions are for generating Table 1
   - Guideline for generating Table 1
   - Set K = 1000 at line 92
   - Set pi = 0.1 at line 132
   - set ndraws = 3000 at line 135
   - set rep = 3000 at line 168
   - set filename 'RC_01_1K.npy' to save simulation data.
   - Then run the following python code to get dataset "RC_or_01_1K.csv" in csv format
        import numpy as np
        arr = np.load("RC_01_1K.npy")
        np.savetxt("RC_or_01_1K.csv", np.transpose(np.concatenate((arr[0],arr[1],arr[2],arr[3]))),fmt='%1.4f', delimiter=",")
   - The entries of the CSV file exactly match the entries of Table 1 in the paper.
3) Running the Code "simu_or_lcfdrn_scth.py": These instructions are for generating Table S1
   - Guideline for generating Table S1
   - Set K = 10000 at line 92
   - Set pi = 0.1 at line 132
   - set ndraws = 500 at line 135
   - set rep = 500 at line 168
   - set filename 'RC_01_10K.npy' to save simulation data.
   - Then run the following python code to get dataset "RC_or_01_10K.csv" in csv format
        import numpy as np
        arr = np.load("RC_01_10K.npy")
        np.savetxt("RC_or_01_10K.csv", np.transpose(np.concatenate((arr[0],arr[1],arr[2],arr[3]))),fmt='%1.4f', delimiter=",")
   - The entries of the CSV file exactly match the entries of Table S1 in the paper.
4) Running the Code "simu_or_lcfdrn_scth.py": These instructions are for generating Table S2
   - Guideline for generating Table S2
   - Set K = 10000 at line 92
   - Set pi = 0.3 at line 132
   - set ndraws = 500 at line 135
   - set rep = 500 at line 168
   - set filename 'RC_03_10K.npy' to save simulation data.
   - Then run the following python code to get dataset "RC_or_03_10K.csv" in csv format
        import numpy as np
        arr = np.load("RC_03_10K.npy")
        np.savetxt("RC_or_03_10K.csv", np.transpose(np.concatenate((arr[0],arr[1],arr[2],arr[3]))),fmt='%1.4f', delimiter=",")
   - The entries of the CSV file exactly match the entries of Table S2 in the paper.
5) Running the Code "simu_or_lcfdrn_scth.py": These instructions are for generating Table S3
   - Guideline for generating Table S3
   - Set K = 1000 at line 92
   - Set pi = 0.3 at line 132
   - set ndraws = 3000 at line 135
   - set rep = 3000 at line 168
   - set filename 'RC_03_1K.npy' to save simulation data.
   - Then run the following python code to get dataset "RC_or_03_1K.csv" in csv format
        import numpy as np
        arr = np.load("RC_03_1K.npy")
        np.savetxt("RC_or_03_1K.csv", np.transpose(np.concatenate((arr[0],arr[1],arr[2],arr[3]))),fmt='%1.4f', delimiter=",")
   - The entries of the CSV file exactly match the entries of Table S3 in the paper.
6) Running the Code "simu_dd_lcfdrn_scth.py": These instructions are for generating Table 2
   - Guideline for generating Table 2
   - Set pi = 0.1 at line 197
   - set filename 'RC_dd_01_15K.npy' to save simulation data.
   - Set pi = 0.3 at line 197
   - set filename 'RC_dd_03_15K.npy' to save simulation data.
   - Then run the following python code to get dataset "RC_dd_03_01_15K.csv" in csv format
        import numpy as np
        arr1 = np.load("RC_dd_03_15K.npy")
        arr2 = np.load("RC_dd_01_15K.npy")
        array_3d =np.array([np.transpose(np.concatenate((arr1[0],arr1[1]))),np.transpose(np.concatenate((arr2[0],arr2[1])))])
        array_2d = array_3d.reshape(-1, array_3d.shape[-1])
        np.savetxt("RC_dd_03_01_15K.csv", array_2d,fmt='%1.4f', delimiter=",")
   - The entries of the CSV file exactly match the entries of Table 2 in the paper.
7) Running the Code "simu_or_compare_lcfdrn_vs_lcfdr.py": These instructions are for generating Table 3
   - Guideline for generating Table 2
   - Set pi = 0.1 at line 197
   - set filename 'RC_dd_01_15K.npy' to save simulation data.
   - Set pi = 0.3 at line 197
   - set filename 'RC_dd_03_15K.npy' to save simulation data.
   - Then run the following python code to get dataset "RC_dd_03_01_15K.csv" in csv format
        import numpy as np
        arr1 = np.load("RC_dd_03_15K.npy")
        arr2 = np.load("RC_dd_01_15K.npy")
        array_3d =np.array([np.transpose(np.concatenate((arr1[0],arr1[1]))),np.transpose(np.concatenate((arr2[0],arr2[1])))])
        array_2d = array_3d.reshape(-1, array_3d.shape[-1])
        np.savetxt("RC_dd_03_01_15K.csv", array_2d,fmt='%1.4f', delimiter=",")
   - The entries of the CSV file exactly match the entries of Table 2 in the paper.
   
