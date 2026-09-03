# DermaScout — Build Status

## Step 1 — Data acquisition: COMPLETE (02 Sep 14:30 IST)
- HAM10000: 10,015 images / 7,470 lesions / 8,659 trainable (nv, akiec, mel, bcc)
- PAD-UFES-20: 2,298 images / 1,373 patients / 1,641 lesions / 1,871 trainable (NEV, ACK, MEL, BCC)
- All 7 HAM and 6 PAD class counts match published values exactly
- Zero rows missing an image; zero placeholder-string group keys; all image IDs unique
- Note: Kaggle HAM archive ships every image twice, byte-identical (deduped at extraction)

## Step 2 — Healthy class (03 Sep 14:17 IST)
- 2,299 crops: 1,128 PAD phone + 1,171 HAM dermoscopic
- surgical ink and dark blobs filtered
- 1,944 unique groups, zero UNKNOWN — leakage-safe

## Step 3 — Master CSV (03 Sep 14:26 IST)
- 13,100 rows, 4 classes
- zero null keys
- two domains

## Step 4a — Dedup (03 Sep 14:59 IST)
- 12,829 images hashed, 0 unreadable
- 1 cross-group duplicate cluster merged

## Step 4a — Dedup (03 Sep 15:11 IST)
- 12,829 images hashed, 0 unreadable
- 1 cross-group duplicate cluster merged

## Step 4a — Dedup (03 Sep 15:13 IST)
- 12,829 images hashed, 0 unreadable
- 1 cross-group duplicate cluster merged

## Step 4 — Split done (03 Sep 15:17 IST)
- 12,829 images deduplicated, 0 unreadable, 1 cross-group duplicate merged
- split 8998 train / 1259 val / 2572 test
- all 4 classes and both domains present in every split
- cancer test set = 538 images

## Step 4 — Split done (03 Sep 15:20 IST)
- 12,829 images deduplicated, 0 unreadable, 1 cross-group duplicate merged
- split 8998 train / 1259 val / 2572 test
- all 4 classes and both domains present in every split
- cancer test set = 538 images
