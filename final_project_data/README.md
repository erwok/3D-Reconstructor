# File Structure Description
## `images` Folder
- Contains the 49-image dataset. Index starts from 0. Notice that every two neighboring images (image `i` and `i+1`) are also photoed by neighboring cameras, meaning that you are able to derive a relatively clean correspondence from every two neighbor images.

## `intrinsics.npy`
- Contains $49 \times 3 \times 3$ numpy array
- `intrinsics[i]` is the $3 \times 3$ intrinsic matrix of camera `i`, corresponding to image of index `i`

## `extrinsics.npy`
- Contains $49 \times 4 \times 4$ numpy array
- `extrinsics[i]` is the $4 \times 4$ extrinsic matrix of camera `i`, corresponding to image of index `i`