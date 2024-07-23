# Inhabitants-of-the-seasStart:
Display "Whale DNA Sequence Simulation"

Define DNA_SEQUENCE_LENGTH = 100  // Length of the DNA sequence
Define DNA_BASES = ['A', 'T', 'C', 'G']  // Possible DNA bases

Function generateRandomDNASequence():
    sequence = ""
    Repeat DNA_SEQUENCE_LENGTH times:
        randomIndex = Random number between 0 and 3  // Select random base index
        base = DNA_BASES[randomIndex]  // Get a random base
        Append base to sequence
    Return sequence

Function displayDNA(sequence):
    Display "DNA Sequence: " + sequence

// Main program
sequence1 = generateRandomDNASequence()
sequence2 = generateRandomDNASequence()

Display "First Whale DNA Sequence:"
displayDNA(sequence1)

Display "Second Whale DNA Sequence:"
displayDNA(sequence2)

End
