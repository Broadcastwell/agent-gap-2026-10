# v1.0.1: preserve the frozen CSV bytes

The first v1.0 archive preserved every row but Git normalized CRLF line endings to LF. As a result, the archived vendor and repeat selection files did not match their pre-run SHA256 hashes byte for byte.

Version v1.0.1 restores the original CSV bytes and marks CSV files as exempt from text normalization. The 70-vendor selection, ten-vendor repeat sample, 240 session rows, scores, dates, unknown values and all reported figures are unchanged. The original v1.0 release and DOI remain available as the dated publication record.

The corrected files must match these frozen hashes:

- AGENT_GAP_SET.csv: a11035069a3cd90fbcff98de56c28cdef82561ec1ec08b633723e044ad041299
- AGENT_GAP_REPEAT_SET.csv: 4e4d6ab02ad56a1ff8e2522eb6dad32719f4719a8d1b0a683844cdd9fb0c6e40

The original data CSV SHA256 is d10ce9a6e01771f7a7428bde89497cd29a21fafbe198ede4ca5b09f440c00fff. A parsed-row comparison also confirms that v1.0 and v1.0.1 contain identical data.
