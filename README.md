sample
===

select #use("cols")# from user_info where #use("condition")#

cols
===
        `user_id`,
        `user_name`,
        `status`,
        `create_time`

updateSample
===
        `user_id=#userId#`,
        `user_name=#userName#`,
        `status=#status#`,
        `create_time=#createTime#`

condition
===
    1 = 1
    @if(!isEmpty(userId)){
      and `user_id`=#userId#
    @}
    @if(!isEmpty(userName)){
      and `user_name`=#userName#
    @}
    @if(!isEmpty(status)){
      and `status`=#status#
    @}
    @if(!isEmpty(createTime)){
      and `create_time`=#createTime#
    @}# New-repository
New repository
