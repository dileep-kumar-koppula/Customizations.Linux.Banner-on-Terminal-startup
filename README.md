# Create Banner for Terminal when it 

## Installing required packages

+ Installations

   ```bash
   sudo apt insatall figlet lolcat neofetch -y
   ```

## Basic Commands for `figlet` and `lolcat`

1. Display a title

   ```bash
   figlet "Title"
   ```

3. Center the title

   ```bash
   figlet -c "Title" | lolcat
   ```

4. Use a specific font to center the title

   ```bash
   figlet -f slant -c "Title" | lolcat
   ```
   
6. Use a different font to display the title

   ```bash
   figlet -f digital "Title" | lolcat
   ```

8. Display a centered title and a message indicating access granted

   ```bash
   figlet -f slant -c "Dileep Kumar" | lolcat && figlet -f digital -c "Access Granted !!" | lolcat
   ```

# Figlet Command Options

## Command Options

- `-c`: Center the Text
- `-f`: Specify the Font

## Available Fonts

The following fonts are available for use with `figlet`:

- `banner.flf`
- `big.flf`
- `block.flf`
- `bubble.flf`
- `digital.flf`
- `ivrit.flf`
- `lean.flf`
- `mini.flf`
- `mnemonic.flf`
- `script.flf`
- `shadow.flf`
- `slant.flf`
- `small.flf`
- `smscript.flf`
- `smshadow.flf`
- `smslant.flf`
- `standard.flf`
- `term.flf`
