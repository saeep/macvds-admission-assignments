# macvds-admission-assignments
Solutions to the MaCV&amp;DS scientific programming admission assignments (Python)

Exercise 1: Set Indexing Bug
Problem: Sets in Python are unordered - indexing gives unpredictable results.
Fix: Convert set to sorted list for deterministic ordering:

Exercise 2: Coordinate Swap Bug
Problem: Simultaneous assignment overwrites values before they can be swapped.
Fix: Create a temporary copy first

Exercise 3: CSV Plotting Bug
Problem: CSV reader returns strings, not floats. Also axes were reversed.
Fix: Convert to floats and correct axis order

Exercise 4: GAN Training Bug
Problem: Last batch in epoch may have fewer samples than `batch_size`, causing tensor dimension mismatch.
Fix: Use the actual batch size from the data (`current_batch_size = real_samples.size(0)`) for all label tensors and latent vectors, and adjust subplot indexing/layout for correct visualization.

