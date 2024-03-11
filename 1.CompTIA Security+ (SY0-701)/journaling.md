Writing data to a journal before writing it to storage 

- Normally, If Power goes out while writing data to storage could result in corrupted data/files
- However, If power goes out while journal is writing to storage then once power is reactivated the corruption will be overwritten with the journal entry.
- Can utilizes atomic transactions so either a transaction is fully carried out or not carried out at all so if power outage occurs during data being written to journal there won't be any corrupted data as there will be no data at all in the journal.