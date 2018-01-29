# AndroidSplitResFolder


### Step 1:
Select Project (instead of Android) (because it make easy to see the project structure)

### Step 2
Right click `res` folder -> `Directory` -> create directory name **layouts**

### Step 3
Right click **layouts** -> `New Folder` -> `Res Folder` -> Check `Change folder location` then create folder name like `src/main/res/layouts/home`

### Step 4
Right click **home** -> New Directory -> **layout**

### Step 5
Right click on **layout** -> create new xml file

### Step 6
Done


## Some note
- You can also create `'menu', 'drawable', 'anim'` inside **home**
- After we split res folder, build gradle will generate like
```
android {
    ...
    sourceSets {
        main {
            res.srcDirs = ['src/main/res', 'src/main/res/layouts/home', 'src/main/res/layouts/setting']
        }
    }
}
```