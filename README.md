Reading Commit Messages

Each commit follows the format: provenance:
YYYY-MM-DD - N receipts (root: XXXXXXXX)

N receipts = Number of file access events (API requests) in this batch

root = Hash binding all receipts for tamper detection

Receipts are batched every ~5 minutes. One commit may contain 1-100+ individual file access records, each with its own cryptographic signature and timestamp.
