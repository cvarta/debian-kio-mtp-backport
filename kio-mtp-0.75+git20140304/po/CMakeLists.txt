# The pofiles macro creates in some versions same name targets
# which since cmake 2.8 leads to target clashes.
# Hence force the old policy for all po directories.
# http://public.kitware.com/Bug/view.php?id=12952
cmake_policy(SET CMP0002 OLD)

find_package(Gettext REQUIRED)
if (NOT GETTEXT_MSGMERGE_EXECUTABLE)
MESSAGE(FATAL_ERROR "Please install msgmerge binary")
endif (NOT GETTEXT_MSGMERGE_EXECUTABLE)
if (NOT GETTEXT_MSGFMT_EXECUTABLE)
MESSAGE(FATAL_ERROR "Please install msgmerge binary")
endif (NOT GETTEXT_MSGFMT_EXECUTABLE)
add_subdirectory(de)
add_subdirectory(pt)
add_subdirectory(el)
add_subdirectory(fr)
add_subdirectory(sk)
add_subdirectory(pt_BR)
add_subdirectory(fi)
add_subdirectory(ru)
add_subdirectory(uk)
add_subdirectory(gl)
add_subdirectory(ga)
add_subdirectory(hu)
add_subdirectory(pl)
add_subdirectory(lt)
add_subdirectory(sl)
add_subdirectory(sv)
add_subdirectory(tr)
add_subdirectory(it)
add_subdirectory(bs)
add_subdirectory(et)
add_subdirectory(cs)
add_subdirectory(es)
add_subdirectory(mr)
add_subdirectory(nl)
add_subdirectory(ca)
add_subdirectory(ro)
add_subdirectory(da)
