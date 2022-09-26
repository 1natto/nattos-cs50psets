# Determine lexico level of text

def main():
    # Calling global variables for counting
    global words, sentences, letters
    words, sentences, letters = 1, 0, 0
    # Invoke counting function taking a string as input
    counter(input("Text: "))
    #  Coleman-Liau index
    index = round(0.0588 * letters / words * 100 - 0.296 * sentences / words * 100 - 15.8)
    # Cases
    if index > 16:
        print("Grade 16+")
    elif index < 1:
        print("Before Grade 1")
    else:
        print("Grade " + str(index))

# Counter function


def counter(text):
    # Invoking gloval variables
    global words, sentences, letters
    # For every letters in text
    for i in text:
        # Is alphabetical
        if i.isalpha() == True:
            letters += 1
        match i:
            # Is space
            case " ":
                words += 1
            # Is punctuation
            case ".":
                sentences += 1
            case "?":
                sentences += 1
            case "!":
                sentences += 1

# Calling main


if __name__ == "__main__":
    main()
