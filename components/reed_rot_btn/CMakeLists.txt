set(COMPONENT_SRCS "reed_rot_btn.c")
set(COMPONENT_ADD_INCLUDEDIRS "include")
set(COMPONENT_REQUIRES "ulp driver")
register_component()
set(ulp_app_name "ulp_reed_rot_btn")
set(ulp_s_sources "ulp/reed_rot_btn.S")
set(ulp_exp_dep_srcs "reed_rot_btn.c")
ulp_embed_binary(${ulp_app_name} "${ulp_s_sources}" "${ulp_exp_dep_srcs}")
