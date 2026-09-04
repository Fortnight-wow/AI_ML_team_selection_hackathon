SUBMISSION FOLDER — AI/ML Team Selection (FER challenge)

What to upload in the Google Form (closes 2 PM):
  1. FER_Submission.pdf  -> PDF of the Jupyter notebook (complete training + submission, highest score)
  2. FER_Report.pdf      -> small report (approach, methodology, results, statistics)

Best score (validation):  macro F1 = 0.651 | accuracy = 66.9%
Final predictions:        submission_final.csv (7,178 rows, id,label)

Also included:
  FER_Submission.ipynb   -> the executed notebook itself (same content as the PDF)

How the score was reached: pretrained ResNet18 fine-tuned at 96x96 (2 seeds),
plus a small CNN baseline and ResNet18@48, combined with an F1-weighted
ensemble and test-time augmentation. No test-set lookahead: the test set was
used once, at the end, only to write predictions.
