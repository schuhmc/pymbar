# MBAR analysis of single-molecule DNA hairpin single-molecule equilibrium experiments under constant force load.

## References

[1] Woodside MT, Behnke-Parks WM, Larizadeh K, Travers K, Herschlag D, and Block SM. Nanomechanical measurements of the sequence-dependent folding landscapes of single nucleic acid hairpins. PNAS 103(16):6190-6195, 2006.

[2] Greenleaf WJ, Woodside MT, Abbondanzieri EA, and Block SM. Passive all-optical force clamp for high-resolution laser trapping. PRL 95:208102, 2005.

## Manifest

* `original-data/` - original data in Excel spreadsheet form, provided by Michael T. Woodside <Michael.Woodside@nrc-cnrc.gc.ca>, corresponding author of [1].  Data has been compressed with bzip2 as `20R55_4T_data.xls.bz2`
* `processed-data/` - external biasing forces (in pN) and extension trajectories (in nm, 0.1 ms time resolution) extracted from the Excel files in original-data/
* `extract-data.py` - Python script to extract data from Excel datafiles (run as `extract_data.py` in place)
* `force-bias-optical-trap.py` - Python script to compute potentials of mean force (PMFs) using MBAR
* `plots/` - directory containing plots
* `output/` - directory containing PMFs

## Usage

Correspondence with the corresponding author, Michael T. Woodside, describing the dataset appears below.

    ---------------------------------------------------------------

    Hi John,

    Here are 5s records, with data points every 0.1 ms, recorded at 16
    different forces for the same molecule, hairpin 20R55/4T in the naming
    scheme I used in the paper. It's the same hairpin as for Fig. 1. I stuck
    the data in an Excel file.

    As far as errors go, there are some reasonably large systematic errors
    that can crop up in the force, so the absolute force values are known to
    within about 10% or so for a given molecule (bead size variations are a
    large factor here). As a first pass, by all means feel free to ignore
    the errors, but it's a good idea to keep them in mind for further down
    the road. Definitely, the file does not quote significant digits
    properly!!

    I have three more datasets that are ready to be sent, and several more
    to sort through. Hopefully this will give you something to work with for
    now...

    Cheers,

    --Michael

    ---------------------------------------------------------------
    Michael Woodside
    National Institute for Nanotechnology, NRC
    and Dept. of Physics, University of Alberta
    ---------------------------------------------------------------

