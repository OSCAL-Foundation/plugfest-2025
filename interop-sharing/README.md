# Interoperability Testing Instructions

Anyone can download the contents of this repository and test tools using the OSCAL files within. We ask that participants follow the instructions below so that we can meaningfully capture the results.

## To share files
Any entity that would like to share their OSCAL content should follow the below instructions:

1. Fork this repository and create a local clone.
2. Add a subfolder with an identifiable name to this folder (if I was representing "ExampleCo", perhaps "interop-sharing/exampleco").
3. Populate the folder with OSCAL files. 
    - *NOTE*: If you cannot upload the files you'd like to share, provide links to the files in your results tracker (see below)
    - Try to keep organization as flat/simple as possible for ease of use (many tools ingest through command-line interfaces).
5. Create a results tracker markdown file for others to track their results ([see template here!](./results-tracker-template.md))
    - Recommended: provide a copy-pastable results entry (see template for example)
6. Submit a PR.

## To test files
1. Fork this repository and create a local clone.
2. Open the results matrix for the organization whose files you'd like to test.
3. Create (or copy) a new section for your tool in the results tracker
4. For each file, record your results.
    - Provide details if possible: what errors were thrown? Is something missing from the file? Is the file valid but not structured or constructed how you or your tool expected?
5. Submit a PR.
