# convert-ttf-to-json
# What is it?

A Python project based on fontTools that can convert TTF font files into JSON files for use in three.js scenes. It supports subsetting font files based on the required characters.

# How to use

1. Provide the font file path "font_file" and the output json file path "json_file". 

   ```shell
   python3 convert_ttf_to_json.py --font_file ./msyh.ttf --json_file ./msyh.json
   ```

2. The "words" parameter can be optionally provided to convert only the necessary text and simplify the output json file. 

   ```shell
   python3 convert_ttf_to_json.py --font_file ./msyh.ttf --json_file ./msyh.json --words abcdefg
   ```

3. The "from_file" parameter can be optionally provided to obtain the text to be converted from a file. When both the "words" parameter and the "from_file" parameter are provided, the "from_file" parameter will be ignored.

   ```shell
   python3 convert_ttf_to_json.py --font_file ./msyh.ttf --json_file ./msyh.json --from_file ./words.txt
   ```

   

