# AI in Medical Imaging(MRI)

The goal of this project is to speed up the MRI machine by sampling the least number of points in the frequency domain. 

# Loading the data

The MRI data are stored in .h5 files, which consists of multiple slices per scan. Only single coil data will be used for the analysis. You can use the DataLoader class to read in the data like:
```
dataloader = DataLoader()
kspace, reconstructed = dataloader.load_data(file_path, # of scans)
```

You can also visualize both the array above like:
```
dataloader.show_slices(kspace, reconstructed)
```

This will show the kspace slice and reconstructed slice of data side-by-side


