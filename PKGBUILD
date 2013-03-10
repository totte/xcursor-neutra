# Maintainer: totte <totte@tott.es>
# PKGBUILD for building the Neutra xcursor theme from a local repository.
# Run 'git clean -dfx' and 'git reset --hard HEAD' to clean up afterwards.
pkgname=xcursor-neutra
pkgver=1.0.0
pkgrel=1
pkgdesc="Personal modification of the Neutral X11 cursor theme"
arch=("any")
url="http://www.tott.es"
license=("PerlArtistic")
depends=()
makedepends=("xorg-xcursorgen")
conflicts=()
options=()

build()
{
  rm -rf cursors
  mkdir cursors
  cp -r ../source ./
  cd source
  for file in *.in; do
    xcursorgen "$file" "../cursors/`basename \"$file\" .in`"
  done
  cd ../cursors
  ln -s circle            03b6e0fcb3499374a867c041f52298f0
  ln -s circle            crossed_circle
  ln -s circle            dnd-no-drop
  ln -s circle            forbidden
  ln -s circle            not-allowed
  ln -s cross             cross_reverse
  ln -s cross             diamond_cross
  ln -s dotbox            dot_box_mask
  ln -s dotbox            draped_box
  ln -s dotbox            icon
  ln -s dotbox            target
  ln -s dnd-copy          1081e37283d90000800003c07f3ef6bf
  ln -s dnd-copy          6407b0e94181790501fd1e167b474872
  ln -s dnd-copy          b66166c04f8c3109214a4fbd64a50fc8
  ln -s dnd-copy          copy
  ln -s dnd-link          3085a0e285430894940527032f8b26df
  ln -s dnd-link          640fb0e74195791501fd1ed57b41487f
  ln -s dnd-link          a2a266d0498c3104214a47bd64ab0fc8
  ln -s dnd-link          alias
  ln -s dnd-link          link
  ln -s dnd-move          4498f0e0c1937ffe01fd06f973665830
  ln -s dnd-move          9081237383d90e509aa00f00170e968f
  ln -s dnd-move          move
  ln -s hand2             9d800788f1b08800ae810202380a0822
  ln -s hand2             e29285e634086352946a0e7090d73106
  ln -s hand2             hand
  ln -s hand2             hand1
  ln -s hand2             pointer
  ln -s hand2             pointing_hand
  ln -s fleur             closedhand
  ln -s fleur             fcf21c00b30f7e3f83fe0dfd12e71cff
  ln -s fleur             openhand
  ln -s fleur             all-scroll
  ln -s fleur             size_all
  ln -s left_ptr          arrow
  ln -s left_ptr          dnd-none
  ln -s left_ptr          top_left_arrow
  ln -s left_ptr_watch    00000000000000020006000e7e9ffc3f
  ln -s left_ptr_watch    08e8e1c95fe2fc01f976f1e063a24ccd
  ln -s left_ptr_watch    3ecb610c1bf2410f44200f48c40d3599
  ln -s left_ptr_watch    half-busy
  ln -s left_ptr_watch    progress
  ln -s left_ptr_watch    watch
  ln -s left_ptr_watch    wait
  ln -s question_arrow    5c6cd98b3f3ebcb1f9c7f1c204630408
  ln -s question_arrow    d9ce0ab605698f320427677b458ad60b
  ln -s question_arrow    dnd-ask
  ln -s question_arrow    help
  ln -s question_arrow    left_ptr_help
  ln -s question_arrow    whats_this
  ln -s right_ptr         draft_large
  ln -s right_ptr         draft_small
  ln -s top_right_corner  fcf1c3c7cd4491d801f1e1c78f100000
  ln -s top_right_corner  fd_double_arrow
  ln -s top_right_corner  size_bdiag
  ln -s top_left_corner   bd_double_arrow
  ln -s top_left_corner   c7088f0f3e6c8088236ef8e1e3e70000
  ln -s top_left_corner   size_fdiag
  ln -s sb_h_double_arrow 028006030e0e7ebffc7f7070c0600140
  ln -s sb_h_double_arrow 14fef782d02440884392942c11205230
  ln -s sb_h_double_arrow h_double_arrow
  ln -s sb_h_double_arrow e-resize
  ln -s sb_h_double_arrow left_side
  ln -s sb_h_double_arrow right_side
  ln -s sb_h_double_arrow row-resize
  ln -s sb_h_double_arrow size_hor
  ln -s sb_h_double_arrow split_h
  ln -s sb_h_double_arrow w-resize
  ln -s sb_up_arrow       up_arrow
  ln -s sb_up_arrow       center_ptr
  ln -s sb_up_arrow       centre_ptr
  ln -s sb_v_double_arrow 00008160000006810000408080010102
  ln -s sb_v_double_arrow 2870a09082c103050810ffdffffe0204
  ln -s sb_v_double_arrow base_arrow_down
  ln -s sb_v_double_arrow base_arrow_up
  ln -s sb_v_double_arrow based_arrow_down
  ln -s sb_v_double_arrow based_arrow_up
  ln -s sb_v_double_arrow bottom_side
  ln -s sb_v_double_arrow col-resize
  ln -s sb_v_double_arrow n-resize
  ln -s sb_v_double_arrow s-resize
  ln -s sb_v_double_arrow size_ver
  ln -s sb_v_double_arrow split_v
  ln -s sb_v_double_arrow top_side
  ln -s sb_v_double_arrow v_double_arrow
  ln -s X_cursor          pirate
  ln -s xterm             ibeam
  ln -s xterm             text
}

package()
{
  install -dm755 "$pkgdir"/usr/share/icons/Neutra
  cp -r "$srcdir"/source/index.theme "$pkgdir"/usr/share/icons/Neutra
  cp -r "$srcdir"/cursors "$pkgdir"/usr/share/icons/Neutra
}
