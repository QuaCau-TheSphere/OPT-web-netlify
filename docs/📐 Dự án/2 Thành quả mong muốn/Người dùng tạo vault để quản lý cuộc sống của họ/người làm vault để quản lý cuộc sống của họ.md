---
share: true
tags:
  - file_thành-quả
  - tt_đang-làm
  - đct_cao
---

%%
#file/thành-quả
%%
Trạng thái:: #tt/đang-làm
Độ cấp thiết:: #đct/cao
Đối tượng thụ hưởng:: [[../../4 Các bên liên quan/Loại đối tượng/Theo nhu cầu/Người muốn quản lý cuộc sống cá nhân|Người muốn quản lý cuộc sống cá nhân]]

Phục vụ cho thành quả:
```dataview
List 
From #file/thành-quả 
where contains(thành-quả-cần-có,[[]]) or contains(thành-quả-hỗ-trợ,[[]]) 
```
Thành quả cần có:: 

Thành phẩm:: 


```dataview
list thành-quả-cần-có[0][0] 
from "📐 Dự án hỗ trợ người mới học Obsidian/6 Kế hoạch" 
```

```dataviewjs
dv.span(dv.pages('"📐 Dự án hỗ trợ người mới học Obsidian/6 Kế hoạch"')["Thành quả cần có"][0][0])
```
