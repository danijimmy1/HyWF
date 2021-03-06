# HyWF_dataset

This folder contains the dataset gathered for the paper Protecting against Website Fingerprinting with Multihoming, published at PoPETS 2020.

It consists in real Tor traces gathered with different single path and multipath algorithms. The files consist in timestamp and direction (incoming or outgoing) of the Tor cells.
More details about the architecture can be found in the paper.

The traces are split in several files to fit GitHub's limit of 100MB:

single-path TCP: tcp-wifi_cells.tar.gz (paths 1 and 2)

HyWF #1: mptcp-hywf_wifiwifi_cells.tar.gz (paths 1 and 2)

HyWF #2: mptcp-hywf_wifiwifi_2_p1_cells.tar.gz (path 1) and mptcp-hywf_wifiwifi_2_p2_cells.tar.gz (path 2)

MPTCP default: mptcp-def_wifiwifi_p1_1_cells.tar.gz and mptcp-def_wifiwifi_p1_2_cells.tar.gz (path 1) and mptcp-def_wifiwifi_p2_cells.tar.gz (path 2)

MPTCP round-robin: mptcp-rr_wifiwifi_p1_cells.tar.gz (path 1) and mptcp-rr_wifiwifi_p2_cells.tar.gz (path 2)

To extract the cell files, run
$ tar -xvf FILE_NAME.tar.gz

The files consist in a pair timestamp - direction of all Tor cells.

The other datasets used in the paper (Wang, Hayes and DF) can be found with the paper in which they were decribed.
