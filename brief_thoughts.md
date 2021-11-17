# Data required
- metadata
  - field metadata
    - sampling type
    - sampling effort
      - dates
      - locations
      - durations, number of traps, etc
  - labwork metadata
    - extraction protocol and kit
    - PCR primers used (info on other reagents preferred)
    - Library preparation information
    - Sequencer used and appropriate parameters
  - bioinformatics metadata
    - demultiplexing strategy, if appropriate
    - primer and adaptor removal
    - denoising and/or clustering strategy
    - taxonomic assignment process, if any
      - algorithm
      - reference library
- core data
  - raw sequencing files (probably demultiplexed, depending on sequencer)
  - adjacency list, with uids to tie sequences to the sample which provided them

The metadata would be highly encouraged, but odds are few would ever comprehensively provide it. The important thing is that they provide enough metadata for the core data to be meaningful for people other than them.

# Key issues
- Reproducibility:
  - Software goes out of date and out of maintenance, even if appropriate conda environment protocols are followed etc. Use of docker containers or VMs etc must be encouraged, but to do so will require quality tutorials
