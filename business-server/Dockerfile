#####################################################################################
# Product: ADempiere gRPC Business Data Server                                      #
# Copyright (C) 2020 Edwin Betancourt                                               #
# Contributor(s): Edwin Betancourt EdwinBetanc0urt@outlook.com                      #
# This program is free software: you can redistribute it and/or modify              #
# it under the terms of the GNU General Public License as published by              #
# the Free Software Foundation, either version 3 of the License, or                 #
# (at your option) any later version.                                               #
# This program is distributed in the hope that it will be useful,                   #
# but WITHOUT ANY WARRANTY; without even the implied warranty of                    #
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the                     #
# GNU General Public License for more details.                                      #
# You should have received a copy of the GNU General Public License                 #
# along with this program.  If not, see <https://www.gnu.org/licenses/>.            #
#####################################################################################
FROM openjdk:8-jre-alpine

WORKDIR /opt/Apps/ADempiere-gRPC-Server/bin/

ENV TYPE business

COPY ./${TYPE}.yaml /opt/Apps/ADempiere-gRPC-Server/bin/${TYPE}_connection.yaml

CMD sh adempiere-${TYPE}-server ./${TYPE}_connection.yaml
