# Docker file for Neovim Open JDK 17 (Java 17) development.
#
# @author Maciej Bedra

# Base Neovim image.
FROM mashmb/nvim-ojdk17:dev

# Install sdkman 
RUN apt-get update
RUN rm /bin/sh && ln -s /bin/bash /bin/sh
RUN apt-get -q -y install curl zip unzip
RUN curl -s https://get.sdkman.io | bash
RUN chmod a+x "$HOME/.sdkman/bin/sdkman-init.sh"
RUN source "$HOME/.sdkman/bin/sdkman-init.sh"
CMD ["nvim", "/root/workspace"]


