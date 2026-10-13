# Analysis plan and acceptance checklist

## Structural (T1w)
- [ ] Original vs skull-stripped T1w images and extraction QC
- [ ] GM/WM/CSF segmentation maps and QC
- [ ] MNI registration and before/after overlay plots

## Functional (LR language run)
- [ ] Verify orientation, space, TR, number of volumes and existing preprocessing
- [ ] Motion correction and FD plot + comments on irregular volumes
- [ ] Gaussian smoothing: justified FWHM, before/after one-volume plots
- [ ] fMRI-to-anatomical MNI overlay and reasoned discussion about avoidable step

## GLM
- [ ] Design matrix based on supplied CSV and HRF
- [ ] Regressor correlation matrix
- [ ] Maps for story and math effects
- [ ] Story-minus-math contrast vector and map
- [ ] Network/atlas interpretation and semantic-literature comparison
- [ ] Theoretical answers

## ICA (variant 2)
- [ ] One timepoint = one sample; fMRI matrix T x voxels
- [ ] Choose component count and explain
- [ ] Spatial maps separately, AXIAL ONLY
- [ ] Correlate first 10 component time courses in algorithm order with appropriate GLM regressors
- [ ] Theoretical answers

## Final
- [ ] Report <=5 pages + 1 appendix page, Arial 11, single column
- [ ] Member contributions + AI use statement
- [ ] 4-5 min Zoom video, all five contribute
- [ ] Confirm presentation recording filename/format discrepancy
- [ ] Submission naming and no extra data/images
