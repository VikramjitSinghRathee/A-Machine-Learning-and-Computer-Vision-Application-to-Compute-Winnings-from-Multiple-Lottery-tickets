# OCR Application to Robustly Extract Winnings from Multiple Lottery Tickets in _One Shot_
It hands-off application that runs text recognition on the ticket pictures, for e.g. taken with a smartphone, to extract the ticket values (Lottery type, draw date, numbers, and multiplier). It then compares them to the winning numbers drawn on the draw date to determine the prize ($).

- User simply needs to pass in the ticket images to the application and it will extract the information on the ticket such as lottery type (whether it is Mega Millions or Powerball), draw date, five 2-digit numbers, 2-digit ball numbers and multiplier WITHOUT any user input.
- It computes matches with the drawn winning number and the prizes (in $) by utilizing the extracted information from the ticket pictures.
- Socrata API was utilized to obtain Mega Millions and Powerball dataset containing previous winning numbers
- It can handle tickets that contain a single set of lottery numbers AND  multiple sets of 5 lottery numbers.
- Instead of user passing as input one ticket image at a time to the application, the user can simply pass a ONE folder containing several ticket pictures and all of them will processed and checked for prizes.
- The current version supports only Powerball and Mega Millions lottery tickets.
- Though not a strict requirement, it is recommended the user takes picture of the lottery ticket as shown in 'BestWay_of_Taking_Photos_EXAMPLE.png'. The application works accurately when the picture is taken of the content between the black lines on the lottery ticket. The green arrows indicate these black lines in the current figure.
- GPU utilized - Tesla V100-SXM2 GPU with 16 GB memory
