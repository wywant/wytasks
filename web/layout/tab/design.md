#Description  
  TabItem是一个Anchor, 点击Anchor触发javascript去控制对应content的显示 
  对应TabContent
#Tab Composite Design  
  * Tabs  
  * TabItemContainer ul   
  * TabItem          li a  li有id, a有href="#idPrefix" 
  * Tab_Container    div  有id
  * Tab_Content      div  有id

##基本流程
  TabItem有active的class, 显示为选中的
  TabConten默认不显示， 当状态为active的时候，设置为显示 
  点击anchor,获取#idPrefix，找到TabItem的li和TabContent的div，设置他们的状态为active  
  
##CSS部分  


##Javascript部分  
###构造函数  
  * tabs的id 用于为anchor加listener
  
  * 



