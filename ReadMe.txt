1. The notebook "MF-Submit.ipynb" implements matrix factorization via the keras layer "Embedding".  
2. We create a latent space consisting of 10 features.  There are 53424 users and 10000 books in the .csv files.  Clearly 10 may be too small, but given the RMSE is around 0.8 it seems to work quite well.
3. When you run the notebook, all the code executes to the 'end' (so the notebook isn't divided into 'blocks').  Once you run it, it loads the .csv files, creates the model, fits the model, displays RMSE value, shows several of the predictions for the test set, and then asks you if you want to see predictions for a particular user.
4.  To get predictions for a particular user, you will see the input box (as shown below)

Enter a user-id from 1 to 53424  (0 to 'quit'): 5000.

Once you enter a valid user-id (like 5000), you will be given a list of books that this user will 'LOVE' (a predicted rating of 4.00 to 4.99), a list of books the user will 'LIKE' (a predicted rating of 3.00 to 3.99), a list of books the user will consider 'SO-SO', 'DISLIKE', and 'HATE'.

5. An example output is shown below (for user 5000)

-----------------------------------------------------------------------------

Books User  5000  will LOVE

The Windup Girl                                                         4.57
Wake (Wake, #1)                                                         4.52
West with the Night                                                     4.50
The Firm (Penguin Readers, Level 5)                                     4.48
Harry Potter Boxset (Harry Potter, #1-7)                                4.48
Dark Fire (Dark, #6)                                                    4.46
Matilda                                                                 4.45
The Red Tent                                                            4.44
Carter Reed (Carter Reed, #1)                                           4.44
Queen of Shadows (Throne of Glass, #4)                                  4.43

-----------------------------------------------------------------------------

Books User  5000  will LIKE

The Mermaid Chair                                                       3.99
Make Way for Ducklings                                                  3.99
Tall, Tatted and Tempting (The Reed Brothers, #1)                       3.99
A Game of Thrones: The Graphic Novel, Vol. 1                            3.99
Their Eyes Were Watching God                                            3.99
The Incredible Journey                                                  3.99
Twilight (Twilight, #1)                                                 3.99
Catch-22                                                                3.99
The Fires of Heaven (Wheel of Time, #5)                                 3.99
The History of Tom Jones, a Foundling                                   3.99

-----------------------------------------------------------------------------

Books User  5000  will consider 'SO-SO'

Lone Wolf                                                               2.99
The Book Thief                                                          2.99
The Silver Chair (Chronicles of Narnia, #4)                             2.99
Foucault's Pendulum                                                     2.99
Field of Prey (Lucas Davenport, #24)                                    2.99
Dracula (Marvel Illustrated)                                            2.99
Tangerine                                                               2.99
Midwives                                                                2.99
Valley of Silence (Circle Trilogy, #3)                                  2.99
The Girl with the Dragon Tattoo (Millennium, #1)                        2.99

-----------------------------------------------------------------------------

Books User  5000  will DISLIKE

Harry Potter and the Deathly Hallows (Harry Potter, #7)                 1.99
Trainspotting                                                           1.90
Romeo and Juliet                                                        1.88
The Fall of Hyperion (Hyperion Cantos, #2)                              1.87
Running with Scissors                                                   1.77
Ubik                                                                    1.75
Flat-Out Love (Flat-Out Love, #1)                                       1.68
The Invention of Hugo Cabret                                            1.59
The School of Essential Ingredients                                     1.44

-----------------------------------------------------------------------------

Books User  5000  will HATE

Little Women (Little Women, #1)                                         0.86
Life of Pi                                                              0.77
