cmake_minimum_required(VERSION 2.6)

PROJECT(ubox C)

ADD_LIBRARY(ubox STATIC
  avl.c
  avl-cmp.c
  blob.c
  blobmsg.c
  uloop.c
  usock.c
  ustream.c
  ustream-fd.c
  vlist.c
  utils.c
  safe_list.c
  runqueue.c
  md5.c
)

ADD_LIBRARY(blobmsg_json STATIC
  blobmsg_json.c
)

TARGET_LINK_LIBRARIES(blobmsg_json
  ubox
  json-c
)
