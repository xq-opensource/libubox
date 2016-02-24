cc_library(
  name = 'ubox',
  warning = 'no',
  extra_cppflags = [
    '-Wno-error=sign-compare',
  ],
  export_incs = './include',
  srcs = [
    'avl.c',
    'avl-cmp.c',
    'blob.c',
    'blobmsg.c',
    'uloop.c',
    'usock.c',
    'ustream.c',
    'ustream-fd.c',
    'vlist.c',
    'utils.c',
    'safe_list.c',
    'runqueue.c',
    'md5.c',
  ]
)

cc_library(
  name = 'blobmsg_json',
  warning = 'no',
  extra_cppflags = [
    '-Wno-error=sign-compare',
  ],
  export_incs = './include',
  srcs = [
    'blobmsg_json.c',
  ],
  deps = [
    ':ubox',
    '//json-c:json-c',
  ]
)
