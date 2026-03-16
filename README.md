# wsl2-bitwarden-ssh-agent

Taken from: https://www.rebelpeon.com/bitwarden-ssh-agent-on-wsl2/

1.  On the Windows host, install npiperelay:

        winget install -e --id albertony.npiperelay

2.  Shell into WSL:

        wsl

3.  Install socat in WSL:

        sudo apt install socat

4.  Make sure the script is executable:

        sudo chmod +x wsl2-bitwarden-ssh-agent.sh

5.  Open `~/.bashrc`, and add the following line, replacing `<path_to_script>`:

        source <path_to_script>/wsl2-bitwarden-ssh-agent.sh
