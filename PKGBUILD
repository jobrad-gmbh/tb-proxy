#!/usr/bin/env bash
# -*- coding: utf-8 -*-
# region header
# Copyright Torben Sickert (info["~at~"]torben.website) 16.12.2012

# License
# -------

# This library written by Torben Sickert stand under a creative commons naming
# 3.0 unported license. see http://creativecommons.org/licenses/by/3.0/deed.de
# endregion
pkgname=proxy
pkgver=1.0.15
pkgrel=13
pkgdesc='generic proxy server'
arch=(any)
url=http://torben.website/proxy
license=(CC-BY-3.0)
depends=(bash docker)
source=(base.yaml Dockerfile proxy.service)
md5sums=(SKIP SKIP SKIP)
copy_to_aur=true

package() {
    install -D --mode 755 "${srcdir}/base.yaml" \
        "${pkgdir}/srv/http/proxy/base.yaml"
    install -D --mode 755 "${srcdir}/Dockerfile" \
        "${pkgdir}/srv/http/proxy/Dockerfile"
    install -D --mode 655 "${srcdir}/proxy.service" \
        "${pkgdir}/etc/systemd/system/proxy.service"
}
# region vim modline
# vim: set tabstop=4 shiftwidth=4 expandtab:
# vim: foldmethod=marker foldmarker=region,endregion:
# endregion
