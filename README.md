# Python1
# Problem 1: Widget Pricing

# Get user input for quantity of widgets
quantity = int(input("Enter the quantity of widgets: "))

# Determine the price based on the schedule
if quantity > 10000:
    price = 10
elif 5000 <= quantity <= 10000:
    price = 20
else:
    price = 30

# Calculate extended price, tax, and total
extended_price = quantity * price
tax_rate = 0.07
tax_amount = extended_price * tax_rate
total = extended_price + tax_amount

# Display results
print(f"\nExtended Price: ${extended_price:.2f}")
print(f"Tax Amount: ${tax_amount:.2f}")
print(f"Total: ${total:.2f}")
