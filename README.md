Responsive-framework
====================

Dev:Mr.wong

因工作需要，参考了boostrap框架之后，搭建的轻量级响应式框架。

说明：
   响应式框架栅格为12格，所有布局都以12格为基本单位，间隔20px;

   在所有四个分辨率下都是20px的间隔：1216，1000，720，720以下

   四个分辨率分别对应：

   1216 === 1280+
   1000 === 1024+
   720 === 768+
   720 === 320+

   响应区域样式：
       .rsp_body
       ----用于限定内容区，在.rsp_body下的区域为响应式区

   功能样式：
       .hide_dtHD/.hide_dt/.hide_pad/.hide_ph
       ----将模块设置为仅在指定分辨率下隐藏
       .show_dtHD/.show_dt/.show_pad/.show_ph
       ----将模块设置为仅在指定分辨率下显示
       .no-margin-right 默认为控制dt
       .dtHD_no-margin-right 控制高分辨率
       .pad_no-margin_right 控制pad分辨率
       ----消除右外补白，关键，由于IE不支持CSS3选择器，所以需要这个样式来消除最后一个子元素的外补白。
       .pad/dtHD_margin-right
       ----添加右补白
       .no-margin-bottom
       ----消除最后一个元素的底部外补白

   布局样式
       跨格定位：
       .dtHD_offset_n / .dt_offset_n / .pad_offset_n / .ph_offset_n
       ----n为数字，对应12格，最大值为11

       容器宽度:
       .col_dtHD_n :桌面1216以上
       .col_dt_n:桌面1000-1216之间
       .col_pad_n:平板721-999之间
       .col_ph_n:手机720以下
       ----n为数字，对应12格宽度，最大值为12，即100%

       .row
       ----用于分行并列模块
