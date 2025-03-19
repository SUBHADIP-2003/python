# python electric bill calculator
def calculate_bill(amount):

    if amount < 800:
        tax = 0
    elif amount >= 800 and amount < 1200:
        tax = amount * 0.10
    elif amount >= 1200 and amount < 2000:
        tax = amount * 0.15
    else:
        tax = amount * 0.22
    total_bill = amount + tax
    return total_bill

bill_amount = int(input("Enter the bill amount: "))
total_bill = calculate_bill(bill_amount)
print("Total bill amount:", total_bill)
