# base6666662vv
Identifying First-Time Senders in a Block
new = []
for tx in block.transactions:
    if w3.eth.get_transaction_count(tx["from"]) == 1:
        new.append(tx["from"])
print("New senders:", len(new))
