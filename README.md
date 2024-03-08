import emoji

# Define emoji faces for calculator buttons
buttons = {
    '1️⃣': '1',
    '2️⃣': '2',
    '3️⃣': '3',
    '➕': '+',
    '4️⃣': '4',
    '5️⃣': '5',
    '6️⃣': '6',
    '➖': '-',
    '7️⃣': '7',
    '8️⃣': '8',
    '9️⃣': '9',
    '✖️': '*',
    '0️⃣': '0',
    '➗': '/',
    '🆗': '=',
    '🔄': 'C'
}

# Function to evaluate the expression
def evaluate(expression):
    try:
        result = eval(expression)
        return result
    except:
        return 'Error'

# Main function
def main():
    expression = ''
    while True:
        print('🧮 Calculator 🧮')
        print('---------------')
        print(expression)
        print('---------------')
        for emoji_face, value in buttons.items():
            print(emoji.emojize(f':{emoji_face}:', use_aliases=True), end=' ')
            if value == '=':
                print()
        print()
        
        user_input = input('Enter emoji face: ')
        
        if user_input in buttons:
            if buttons[user_input] == 'C':
                expression = ''
            elif buttons[user_input] == '=':
                result = evaluate(expression)
                print(f'Result: {result}')
                expression = str(result)
            else:
                expression += buttons[user_input]

# Run the program
if __name__ == "__main__":
    main()
