# Create `Banner` to `Terminal` when it opens

## Installing required packages

+ Installations

   ```bash
   sudo apt insatall figlet lolcat neofetch -y
   ```

### Basic Commands for `figlet` and `lolcat`

+ Display a title

   ```bash
   figlet "Title"
   ```

+ Center the title

   ```bash
   figlet -c "Title" | lolcat
   ```

+ Use a specific font to center the title

   ```bash
   figlet -f slant -c "Title" | lolcat
   ```
   
+ Use a different font to display the title

   ```bash
   figlet -f digital "Title" | lolcat
   ```

+ Display a centered title and a message indicating access granted

   ```bash
   figlet -f slant -c "Dileep Kumar" | lolcat && figlet -f digital -c "Access Granted !!" | lolcat
   ```

# Figlet Command Options

## Command Options

   - `-c`: Center the Text
   - `-f`: Specify the Font

## Available Fonts

+ The following fonts are available for use with `figlet`:

   `banner.flf`, `big.flf`, `block.flf`, `bubble.flf`, `digital.flf`, `ivrit.flf`, `lean.flf`, `mini.flf`, `mnemonic.flf`, `script.flf`, `shadow.flf`, `slant.flf`, `small.flf`, `smscript.flf`, `smshadow.flf`, `smslant.flf`, `standard.flf`, `term.flf`

+ You can use them with direct file name (without .flf extension) as

   ```bash
   figlet -f shadow "Title"
   ```

# Neofetch

## Edit Neofetch file

   + Customize however you like by just chnaging values (If you see the file, you will understand)
   
      ```bash
      sudo ${HOME}/.config/neofetch/config.conf
      ```

   + Open other terminal and type `neofetch`. You can view
   + neofetch will continuously run every 1 second

      ```bash
      while neofetch; do sleep 1; done
      ```

# Banner

## Edit the `.bashrc` file to create banner

+ Edit bashrc file

   ```bash
   sudo nano ${HOME}/.bashrc
   ```
   
+ Add the following lines to end of the file

   ```bash
   # Banner with figlet and lolcat
   figlet -c "Dileep Kumar" | lolcat
   
   #Space between above command and below command
   echo ""
   echo ""
   
   # Open Neofetch
   /usr/bin/neofetch
   ```
