# Next Steps

## Current status
- GitHub repository and project documentation are set up.
- Google Colab runs PyTorch and TorchVision on a Tesla T4 GPU.
- MobileNetV2 loads and produces two outputs.
- A training step runs on artificial images and labels.
- No lung-ultrasound videos or patient data have been used.

## What the tests show
The synthetic test confirms that the software workflow executes. It does not
show that the model can identify pneumonia, and its loss and predictions are
not medical results.

## Data-use blocker
COVIDx-US combines data from multiple sources. Its README lists different
license conditions for different sources, including sources with no data-use
license information. Do not download or use source videos until permission for
the specific intended use is verified.

## Next actions
1. Review source-level permissions for any candidate data.
2. If permission is unclear, contact the source or choose another dataset with
   explicit terms that allow the intended research use.
3. Once data use is permitted, document the dataset version, label definitions,
   source attribution, and license in `DATASET.md`.
4. Create patient- or video-level train, validation, and test splits before
   extracting frames.
5. Train and evaluate the model only after the data and split are verified.
6. Record real results in `EXPERIMENT_LOG.md`.

## Safety and scope
This is an educational prototype, not a clinically validated medical device.
Do not use its outputs to diagnose or guide treatment.
