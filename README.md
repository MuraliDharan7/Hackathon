# Registered ticket IDs for particular seats
registered_tickets = {
    "Seat1": "ABC123",
    "Seat2": "DEF456",
    "Seat3": "GHI789"
}

# Function to check if the entered ticket ID is correct for a particular seat
def check_ticket(ticket_id, seat):
    if seat in registered_tickets and registered_tickets[seat] == ticket_id:
        return True
    else:
        return False

# Main program
def main():
    seat = input("Enter the seat number: ")
    ticket_id = input("Enter your ticket ID: ")

    if check_ticket(ticket_id, seat):
        print("Ticket ID is correct. You can sit in Seat", seat)
    else:
        print("Ticket ID is incorrect. Please try again.")
        # Activate red light or display an error message here

# Run the main program
if __name__ == "__main__":
    main()
