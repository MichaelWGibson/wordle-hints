# 12 Days of Christmas - Wordle Hints

A Wordle-style game for revealing Christmas gift hints! This project creates a fun, interactive way to give hints for presents by having the recipient play a Wordle game.

## How It Works

1. Create a comma-separated list of possible hints (5 letters each work best)
2. Base64 encode the list
3. Share a URL with the encoded hints as a parameter
4. The recipient plays Wordle to discover one randomly selected hint

## Usage

### Creating a Hint URL

1. List your hints separated by commas (e.g., "GIFT,TREE,BELLS,SNOWMAN")
2. Base64 encode the string
3. Add it to the URL: `https://yourusername.github.io/wordle-hints/?target=encodedstring`

### Example

For hints: "GIFT,TREE,BELLS,SNOWMAN,MISTLETOE"

Encode to base64: `R0lGVCxUUkVFLEJFTExTLFNOT1dNQU4sTUlTVExFVE9F`

Full URL: `https://yourusername.github.io/wordle-hints/?target=R0lGVCxUUkVFLEJFTExTLFNOT1dNQU4sTUlTVExFVE9F`

### Encoding Base64

You can encode your hints using:

**Command Line (Linux/Mac):**
```bash
echo -n "SCARF,WATCH,BOOTS" | base64
```

**Online Tools:**
- https://www.base64encode.org/

**JavaScript Console:**
```javascript
btoa("SCARF,WATCH,BOOTS")
```

## Features

- Complete Wordle implementation with color-coded letter feedback
- Green: Correct letter in correct position
- Yellow: Correct letter in wrong position
- Gray: Letter not in word
- On-screen keyboard and physical keyboard support
- Responsive design for mobile and desktop
- Randomly selects one hint from your list

## Setting Up GitHub Pages

1. Push this repository to GitHub
2. Go to repository Settings
3. Navigate to Pages section
4. Under "Source", select "Deploy from a branch"
5. Select "main" branch and "/ (root)" folder
6. Click Save
7. Your site will be available at `https://yourusername.github.io/wordle-hints/`

## Tips

- Use 5-letter words for the best Wordle experience
- Words shorter than 5 letters will be padded with spaces
- Words longer than 5 letters will be truncated to 5 letters
- Mix easier and harder hints for variety throughout the 12 days
