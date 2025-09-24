# Challenge Name
an epic file system quest

## My solve
**Flag:** pwn.college{4ta9TtJyZW3QohvPhaKKi_MWmN4.QX5IDO0wyN0gjNzEzW}

```bash
Connected!
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls /
BRIEF  boot       dev  flag  lib    lib64   media  nix  proc  run   srv  tmp  var
bin    challenge  etc  home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~an-epic-filesystem-quest:/$ cat BRIEF
Congratulations, you found the clue!
The next clue is in: /opt/linux/linux-5.4/drivers/dax/pmem

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/$ cd /opt/linux/linux-5.4/drivers/dax/pmem
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/dax/pmem$ ls /opt/linux/linux-5.4/drivers/dax/pmem
Makefile  NUGGET  compat.c  core.c  pmem.c
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/dax/pmem$ cat NUGGET
Yahaha, you found me!
The next clue is in: /opt/linux/linux-5.4/arch/x86/ia32
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/dax/pmem$ cd  /opt/linux/linux-5.4/arch/x86/ia32
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/x86/ia32$ ls  /opt/linux/linux-5.4/arch/x86/ia32
CLUE  Makefile  audit.c  audit.o  built-in.a  ia32_aout.c  ia32_signal.c  ia32_signal.o  sys_ia32.c  sys_ia32.o
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/x86/ia32$ cat CLUE
Congratulations, you found the clue!
The next clue is in: /usr/share/m17n

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/arch/x86/ia32$ cd /usr/share/m17n
hacker@commands~an-epic-filesystem-quest:/usr/share/m17n$ ls -a /usr/share/m17n
.                     IBM424.map           ar.lnm              iu.lnm                    sa.lnm
..                    IBM437.map           as-inscript.mim     ja-anthy.mim              scripts
.SPOILER              IBM500.map           as-itrans.mim       ja-tcode.mim              sd-inscript.mim
8859-10.map           IBM850.map           as-phonetic.mim     ja-trycode.mim            se.lnm
8859-11.map           IBM851.map           as.lnm              ja.lnm                    si-phonetic-dynamic.mim
8859-13.map           IBM852.map           ath-phonetic.mim    ka-kbd.mim                si-samanala.mim
8859-14.map           IBM855.map           az.lnm              ka.lnm                    si-singlish.mim
8859-15.map           IBM857.map           az_Cyrl.lnm         kk-arabic.mim             si-sumihiri.mim
8859-16.map           IBM860.map           az_Latn.lnm         kk-kbd.mim                si-trans.mim
8859-2.map            IBM861.map           be-kbd.mim          kk.lnm                    si-wijesekera.mim
8859-3.map            IBM862.map           be.lnm              kl.lnm                    sid.lnm
8859-4.map            IBM863.map           bg.lnm              km-yannis.mim             sk-kbd.mim
8859-5.map            IBM864.map           bla-phonetic.mim    km.lnm                    sk.lnm
8859-6.map            IBM865.map           bn-disha.mim        kn-inscript.mim           sl.lnm
8859-7.map            IBM866.map           bn-inscript.mim     kn-itrans.mim             so.lnm
8859-8.map            IBM868.map           bn-itrans.mim       kn-kgp.mim                sq.lnm
8859-9.map            IBM869.map           bn-probhat.mim      kn-optitransv2.mim        sr-kbd.mim
ARAB-OTF-NO-GPOS.flt  IBM870.map           bn-unijoy.mim       kn-typewriter.mim         sr.lnm
ARAB-OTF.flt          IBM871.map           bn.lnm              kn.lnm                    sr_Latn.lnm
ARAB.flt              IBM874.map           bo-ewts.mim         ko-han2.mim               ssymbol.mim
BENG-OTF.flt          IBM875.map           bo-tcrc.mim         ko-romaja.mim             sv-post.mim
BIDI.tab              IBM880.map           bo-wylie.mim        ko.lnm                    sv.lnm
BIG5-HKSCS.map        IBM891.map           bs.lnm              kok.lnm                   sw.lnm
BIG5.map              IBM903.map           byn.lnm             ks-inscript.mim           syr.lnm
BLOCK.tab             IBM904.map           ca.lnm              ks-kbd.mim                syrc-phonetic.mim
BNG2-OTF.flt          IBM905.map           cjk-util.mim        ku.lnm                    ta-inscript.mim
CASE-C.tab            IBM918.map           cmc-kbd.mim         kw.lnm                    ta-itrans.mim
CASE-MAPPING.tab      JISX0201.map         cr-western.mim      ky.lnm                    ta-lk-renganathan.mim
CASE-S.tab            JISX0208.map         cs-kbd.mim          latn-post.mim             ta-phonetic.mim
CASED.tab             JISX0212.map         cs.lnm              latn-pre.mim              ta-tamil99.mim
CATEGORY.tab          JISX2131.map         cy.lnm              latn1-pre.mim             ta-typewriter.mim
CHAM-GENERIC.flt      JISX2132.map         da-post.mim         ln.lnm                    ta-vutam.mim
CHARSET.tbl           JISX213A.map         da.lnm              lo-kbd.mim                ta.lnm
CNS-1.map             JOHAB.map            de.lnm              lo-lrt.mim                tai-sonla.mim
CNS-2.map             KA-ACADEMY.map       default.fst         lo.lnm                    te-apple.mim
CNS-3.map             KA-PS.map            dv-phonetic.mim     lsymbol.mim               te-inscript.mim
CNS-4.map             KHMR-ANLONG.flt      dv.lnm              lt.lnm                    te-itrans.mim
CNS-5.map             KHMR-OTF.flt         dz.lnm              lv.lnm                    te-pothana.mim
CNS-6.map             KND2-OTF.flt         el-kbd.mim          mai-inscript.mim          te-rts.mim
CNS-7.map             KNDA-OTF.flt         el.lnm              math-latex.mim            te-sarala.mim
CNS-F.map             KOI-8.map            en.lnm              mdb.dir                   te.lnm
CODING.tbl            KOI8-R.map           eo-h-f.mim          mk.lnm                    tg.lnm
COMBINE.tab           KOI8-T.map           eo-h.mim            ml-enhanced-inscript.mim  th-kesmanee.mim
COMBINING.flt         KOI8-U.map           eo-plena.mim        ml-inscript.mim           th-pattachote.mim
CP10007.map           KSC5601.map          eo-q.mim            ml-itrans.mim             th-tis820.mim
CP1250.map            KSC5636.map          eo-vi.mim           ml-mozhi.mim              th.lnm
CP1251.map            LANGUAGE.tbl         eo-x.mim            ml-remington.mim          ti.lnm
CP1252.map            LAOO-ALICE.flt       eo.lnm              ml-swanalekha.mim         tig.lnm
CP1253.map            LAOO-GENERIC.flt     es.lnm              ml.lnm                    tr.lnm
CP1254.map            LAOO-MULE.flt        et.lnm              mn.lnm                    truetype.fst
CP1255.map            LAOO-OTF.flt         eu.lnm              mr-inscript.mim           tt.lnm
CP1256.map            LINEBREAK.tab        fa-isiri.mim        mr-itrans.mim             ug-kbd.mim
CP1257.map            LOCALE.ali           fa.lnm              mr-phonetic.mim           uk-kbd.mim
CP1258.map            LOCALE.cs            fi.lnm              mr-remington.mim          uk.lnm
CP737.map             MLM2-OTF.flt         fo.lnm              mr-typewriter.mim         unicode.mim
CP775.map             MLYM-CDAC.flt        fr-azerty.mim       mr.lnm                    ur-phonetic.mim
CP949-2BYTE.map       MLYM-OTF.flt         fr.lnm              ms.lnm                    ur.lnm
DEV2-OTF.flt          MLYM-RACHANA.flt     fur.lnm             mt.lnm                    uz-kbd.mim
DEVA-CDAC.flt         MYMR-MYAZEDI.flt     ga.lnm              my-kbd.mim                uz.lnm
DEVA-OTF.flt          MYMR-SIL.flt         generic.fst         nb.lnm                    uz_Arab.lnm
FONTENC.tbl           NAME.tab             gez.lnm             ne-rom-translit.mim       uz_Latn.lnm
FONTSIZE.tbl          NO-CTL.flt           gl.lnm              ne-rom.mim                vi-base.mim
GB180302.map          ORY2-OTF.flt         global.mim          ne-trad-ttf.mim           vi-han.mim
GB180304.map          ORYA-OTF.flt         grc-mizuochi.mim    ne-trad.mim               vi-nom-vni.mim
GB2312.map            SCRIPT-LANGUAGE.tbl  gu-inscript.mim     nl.lnm                    vi-nom.mim
GBK.map               SCRIPT-OTF.tbl       gu-itrans.mim       nn.lnm                    vi-tcvn.mim
GB_1988-80.map        SCRIPT.tab           gu-phonetic.mim     nsk-phonetic.mim          vi-telex.mim
GJR2-OTF.flt          SCRIPT.tbl           gu.lnm              oj-phonetic.mim           vi-viqr.mim
GUJR-OTF.flt          SINH-OTF.flt         gv.lnm              om.lnm                    vi-vni.mim
GUR2-OTF.flt          SOFT-DOTTED.tab      haw.lnm             or-inscript.mim           vi.lnm
GURU-OTF.flt          SYRC-OTF.flt         he-kbd.mim          or-itrans.mim             wal.lnm
HEBR-FF.flt           TAML-CDAC.flt        he.lnm              or-phonetic.mim           xfont.fst
HEBR-OTF.flt          TAML-OTF.flt         hi-inscript.mim     or.lnm                    yi-yivo.mim
HEBR.flt              TEL2-OTF.flt         hi-itrans.mim       pa-anmollipi.mim          zh-bopomofo.mim
IBM037.map            TELU-OTF.flt         hi-optitransv2.mim  pa-inscript.mim           zh-cangjie.mim
IBM038.map            THAA-OTF.flt         hi-phonetic.mim     pa-itrans.mim             zh-pinyin-vi.mim
IBM1004.map           THAI-GENERIC.flt     hi-remington.mim    pa-jhelum.mim             zh-pinyin.mim
IBM1026.map           THAI-NORASI.flt      hi-typewriter.mim   pa-phonetic.mim           zh-py-b5.mim
IBM1047.map           THAI-OTF.flt         hi-vedmata.mim      pa.lnm                    zh-py-gb.mim
IBM256.map            THAI-TIS620.flt      hi.lnm              pl.lnm                    zh-py.mim
IBM273.map            TIBT-MTIB.flt        hr-kbd.mim          ps-phonetic.mim           zh-quick.mim
IBM274.map            TIBT-MULE.flt        hr.lnm              ps.lnm                    zh-tonepy-b5.mim
IBM275.map            TIBT-OTF.flt         hu-rovas-post.mim   pt.lnm                    zh-tonepy-gb.mim
IBM277.map            TIS-620.map          hu.lnm              rfc1345.mim               zh-tonepy.mim
IBM278.map            TML2-OTF.flt         hy-kbd.mim          ro.lnm                    zh-util.mim
IBM280.map            VISCII.map           hy.lnm              ru-kbd.mim                zh-zhuyin.mim
IBM281.map            VSCII.map            icons               ru-phonetic.mim           zh.lnm
IBM284.map            aa.lnm               id.lnm              ru-translit.mim           zh_Hans.lnm
IBM285.map            af.lnm               ii-phonetic.mim     ru-yawerty.mim            zh_Hant.lnm
IBM290.map            am-sera.mim          is.lnm              ru.lnm
IBM297.map            am.lnm               ispell.mim          sa-harvard-kyoto.mim
IBM420.map            ar-kbd.mim           it.lnm              sa-iast.mim
IBM423.map            ar-translit.mim      iu-phonetic.mim     sa-itrans.mim
hacker@commands~an-epic-filesystem-quest:/usr/share/m17n$ cat .SPOILER
Congratulations, you found the clue!
The next clue is in: /opt/busybox/busybox-1.33.2/include/config/feature/lzma

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/share/m17n$ cd  /opt/busybox/busybox-1.33.2/include/config/feature/lzma
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/lzma$ ls -a  /opt/busybox/busybox-1.33.2/include/config/feature/lzma
.  ..  .INSIGHT  fast.h
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/lzma$ cat .INSIGHT
Yahaha, you found me!
The next clue is in: /opt/linux/linux-5.4/drivers/staging/greybus/Documentation/firmware

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/busybox/busybox-1.33.2/include/config/feature/lzma$ cd /opt/linux/linux-5.4/drivers/staging/greybus/Documentation/firmware
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/staging/greybus/Documentation/firmware$ ls /opt/linux/linux-5.4/drivers/staging/greybus/Documentation/firmware
INFO  authenticate.c  firmware-management  firmware.c
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/staging/greybus/Documentation/firmware$ cat INFO
Great sleuthing!
The next clue is in: /usr/share/racket/pkgs/typed-racket-lib/typed-racket/rep/compiled

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/staging/greybus/Documentation/firmware$ cd  /usr/share/racket/pkgs/typed-racket-lib/typed-racket/rep/compiled
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/typed-racket-lib/typed-racket/rep/compiled$ ls  /usr/share/racket/pkgs/typed-racket-lib/typed-racket/rep/compiled
CUE                    core-rep_rkt.dep    free-ids_rkt.zo             prop-rep_rkt.dep    type-mask_rkt.zo
base-type-rep_rkt.dep  core-rep_rkt.zo     free-variance_rkt.dep       prop-rep_rkt.zo     type-rep_rkt.dep
base-type-rep_rkt.zo   filter-rep_rkt.dep  free-variance_rkt.zo        rep-switch_rkt.dep  type-rep_rkt.zo
base-types_rkt.dep     filter-rep_rkt.zo   numeric-base-types_rkt.dep  rep-switch_rkt.zo   values-rep_rkt.dep
base-types_rkt.zo      fme-utils_rkt.dep   numeric-base-types_rkt.zo   rep-utils_rkt.dep   values-rep_rkt.zo
base-union_rkt.dep     fme-utils_rkt.zo    object-rep_rkt.dep          rep-utils_rkt.zo
base-union_rkt.zo      free-ids_rkt.dep    object-rep_rkt.zo           type-mask_rkt.dep
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/typed-racket-lib/typed-racket/rep/compiled$ cat CUE
Tubular find!
The next clue is in: /usr/share/icons/hicolor/72x72/stock/text
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/typed-racket-lib/typed-racket/rep/compiled$ cd /usr/share/icons/hicolor/72x72/stock/text
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/hicolor/72x72/stock/text$ ls /usr/share/icons/hicolor/72x72/stock/text
ALERT
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/hicolor/72x72/stock/text$ cat ALERT
Lucky listing!
The next clue is in: /usr/local/lib/python3.8/dist-packages/jedi/third_party/typeshed/third_party/3/docutils/parsers/rst

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/hicolor/72x72/stock/text$ ls  /usr/local/lib/python3.8/dist-packages/jedi/third_party/typeshed/third_party/3/docutils/parsers/rst
TRACE-TRAPPED  __init__.pyi  nodes.pyi  roles.pyi  states.pyi
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/hicolor/72x72/stock/text$ cat TRACE-TRAPPED
cat: TRACE-TRAPPED: No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/hicolor/72x72/stock/text$ cat  /usr/local/lib/python3.8/dist-packages/jedi/third_party/typeshed/third_party/3/docutils/parsers/rst/TRACE-TRAPPED
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{4ta9TtJyZW3QohvPhaKKi_MWmN4.QX5IDO0wyN0gjNzEzW}
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/hicolor/72x72/stock/text$

```
## Incorrect tangents I went on
i made a mistake in the absolute path in the end. i alse forgot to use cat ls -a a few times

## What I learned
I learned about that this takes extreme patience to perform. I learnt to apply cd,cat,ls, ls -a and absolute paths

## References 
None
