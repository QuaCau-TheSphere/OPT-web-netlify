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
Đối tượng thụ hưởng:: [Người muốn quản lý cuộc sống cá nhân](../../4%20C%C3%A1c%20b%C3%AAn%20li%C3%AAn%20quan/Lo%E1%BA%A1i%20%C4%91%E1%BB%91i%20t%C6%B0%E1%BB%A3ng/Theo%20nhu%20c%E1%BA%A7u/Ng%C6%B0%E1%BB%9Di%20mu%E1%BB%91n%20qu%E1%BA%A3n%20l%C3%BD%20cu%E1%BB%99c%20s%E1%BB%91ng%20c%C3%A1%20nh%C3%A2n.md)  
  
Phục vụ cho thành quả:  
```dataview  
List   
From #file/thành-quả   
where contains(thành-quả-cần-có,[](.md)) or contains(thành-quả-hỗ-trợ,[](.md))   
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
