# ovpn-to-apc.sh
convert an openvpn-configuration to an Astaro / Sophos .apc file

The config file needs to contain the ca, cert and key directives that point to the corresponding files.  

References:

https://ideas.sophos.com/forums/17359-astaro-gateway-feature-requests/suggestions/715890-ssl-vpn-convert-ovpn-to-apc-epc?ref=title

https://community.sophos.com/products/unified-threat-management/astaroorg/f/asg-v7-400-beta-closed/67045/feature-request-7-400-way-to-generate-openvpn-apc-file-for-non-astaro-server

https://community.sophos.com/products/unified-threat-management/f/german-forum/59048/site-to-site-vpn-mit-ovpn-datei
```
##
# ovpn-to-apc.sh
# -----------------------------------------------
# (C) 2009 Patrick Schneider http://goo.gl/5bPqy
# (C) 2012 Stefan Rubner    <stefan@whocares.de>
# (C) 2017 Christoph Loesch       http://chil.at
# -----------------------------------------------
# Changes:
# 2017-11-25
#   Christoph Loesch
#    * Forked repository from https://gitorious.org/admintools/ovpn-to-apc to https://github.com/vchrizz/ovpn-to-apc
#    * minor corrections and two small fixes
# 2012-05-28
#   Stefan Rubner
#    * Added support for 'tls-auth' in old style
#      .ovpn files, too
# 2012-05-26
#   Stefan Rubner:
#    * Started work on making the script work
#      with embedded certs and keys (tnx Alois)
# 2012-04-17
#   Stefan Rubner:
#    * Fixed tr calls to also strip \r in .ovpn
#      files created on Windows
#    * Added some defaults for settings that may
#      not be present in the .ovpn but are needed
#      by the Astaro Security Gateway
#    * reformatted the code a bit and added some
#      comments
# 2009-01-22
#   Patrick Schneider:
#    * initial revision
# -----------------------------------------------
# Usage:
#    ovpn-to-apc.sh $1 $2 [$3 [$4]]
#
# $1 : OpenVPN Config File
# $2 : Astaro .apc to create
# $3 : username
# $4 : password
#
##
```
