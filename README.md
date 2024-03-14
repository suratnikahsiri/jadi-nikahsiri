<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE html>
<html b:css='false' b:version='2' class='v2' expr:dir='data:blog.languageDirection' xmlns='http://www.w3.org/1999/xhtml' xmlns:b='http://www.google.com/2005/gml/b' xmlns:data='http://www.google.com/2005/gml/data' xmlns:expr='http://www.google.com/2005/gml/expr'>
  <head>
    <!--meta expr:content='data:blog.isMobile         ? &quot;width=device-width,initial-scale=1.0,minimum-scale=1.0,maximum-scale=1.0&quot;         : &quot;width=1100&quot;' name='viewport'/-->
    <meta content='width=device-width, initial-scale=1' name='viewport'/>

    <b:include data='blog' name='all-head-content'/>
    <include expiration='7d' path='*.css'/>
    <include expiration='7d' path='*.js'/>
    <include expiration='3d' path='*.gif'/>
    <include expiration='3d' path='*.jpeg'/>
    <include expiration='3d' path='*.jpg'/>
    <include expiration='3d' path='*.png'/>
    <b:if cond='data:blog.pageType == &quot;index&quot;'>
      <title>
        <data:blog.title/>
      </title>
      <b:else/>
      <title>
        <data:blog.pageName/>
      </title>
    </b:if>

        <b:skin><![CDATA[

        
        /*
        -----------------------------------------------
        Blogger Template Style
        Name      : Aroodam Landing Page Template
        Designer  : Aroodam Web & Design
        version   : 2.2.2
        URL       : http://themes.aroodam.com/landing-page/
        ----------------------------------------------- */


        Versi 2.2.2 (24 Mei 2020)
        - Menambahkan pilihan layout header & Menu
        - Menambahkan link title di footer
        - Menampilkan kembali pengaturan Blog Posts Gadget
        - Menampilkan kembali sidebar (gunakan hanya untuk layout Boxed)
        - Perbaikan elemen FAQ hanya 1 yang aktif
        - Perbaikan elemen Pricing-4 dan Pricing-5 agar bisa dipasang lebih dari satu
        - Optimasi tampilan detail lainnya...

        Versi 2.2.1 (29 Oktober 2019)
        - Perbaikan tampilan posting
        - Optimasi kecepatan load

        Versi 2.2 (21 Oktober 2019)
        - Landing Page di Pages & Posts
        - Perbaikan tidak bisa ganti font

        Versi 2.1 (30 April 2019)
        - Perbaikan widget contact form yang tidak bekerja

        Versi 2.0 (1 November 2018)
        - Menjadi 100 elemen

        Versi 1.0 (7 Februari 2017)
        - Rilis


        /* Variable definitions
        ====================
        <Variable name="keycolor" description="Main Color" type="color" default="#66bbdd" value="#adbbd5"/>
        <Group description="Page Text" selector="body">
        <Variable name="body.font" description="Font" type="font"
        default="normal normal 16px Roboto, Arial, Tahoma, Helvetica, FreeSans, sans-serif" value="normal normal 16px Roboto, Arial, Tahoma, Helvetica, FreeSans, sans-serif"/>
        <Variable name="body.text.color" description="Text Color" type="color" default="#333333" value="#494949"/>
        </Group>
        <Group description="Backgrounds" selector=".body-fauxcolumns-outer">
        <Variable name="body.background.color" description="Outer Background" type="color" default="#fbfbfb" value="#fcfcfc"/>
        <Variable name="content.background.color" description="Main Background" type="color" default="#ffffff" value="#ffffff"/>
        <Variable name="header.background.color" description="Header Background" type="color" default="transparent" value="rgba(64,64,64,0)"/>
        </Group>
        <Group description="Links" selector=".main-outer">
        <Variable name="link.color" description="Link Color" type="color" default="#2288bb" value="#2455c6"/>
        <Variable name="link.visited.color" description="Visited Color" type="color" default="#888888" value="#8d8d8d"/>
        <Variable name="link.hover.color" description="Hover Color" type="color" default="#33aaff" value="#3a65ff"/>
        </Group>
        <Group description="Blog Title" selector=".header h1">
        <Variable name="header.font" description="Font" type="font"
        default="normal normal 60px Roboto, Arial, Tahoma, Helvetica, FreeSans, sans-serif" value="normal normal 60px Roboto, Arial, Tahoma, Helvetica, FreeSans, sans-serif"/>
        <Variable name="header.text.color" description="Title Color" type="color" default="#333333"  value="#494949"/>
        </Group>
        <Group description="Blog Description" selector=".header .description">
        <Variable name="description.text.color" description="Description Color" type="color"
        default="#777777"  value="#7d7d7d"/>
        </Group>
        <Group description="Tabs Text" selector=".tabs-inner .widget li a">
        <Variable name="tabs.font" description="Font" type="font"
        default="normal normal 14px Roboto, Arial, Tahoma, Helvetica, FreeSans, sans-serif" value="normal normal 14px Roboto, Arial, Tahoma, Helvetica, FreeSans, sans-serif"/>
        <Variable name="tabs.text.color" description="Text Color" type="color" default="#999999" value="#9d9d9d"/>
        <Variable name="tabs.selected.text.color" description="Selected Color" type="color" default="#000000" value="#000000"/>
        </Group>
        <Group description="Tabs Background" selector=".tabs-outer .PageList">
        <Variable name="tabs.background.color" description="Background Color" type="color" default="rgba(0, 0, 0, 0)" value="rgba(64,64,64,0)"/>
        <Variable name="tabs.selected.background.color" description="Selected Color" type="color" default="rgba(0, 0, 0, 0)" value="rgba(64,64,64,0)"/>
        </Group>

        <!-- ################### -->
        <!-- COVER -->
        <!-- ################### -->
        <Group description="Cover" selector=".cover .w-cover h2">
        <Variable name="cover.font" description="Font" type="font"
        default="normal normal 48px Roboto, Arial, Tahoma, Helvetica, FreeSans, sans-serif" value="normal normal 48px Roboto, Arial, Tahoma, Helvetica, FreeSans, sans-serif"/>
        <Variable name="cover.background.color" description="Background Color" type="color" default="#367ABD" value="#384cc6"/>
        <Variable name="cover.text.color" description="Title Color" type="color" default="#ffffff"  value="#ffffff"/>
        </Group>

        <!-- ################### -->
        <!-- PEMISAH 1 -->
        <!-- ################### -->
        <Group description="Pemisah 1" selector=".aroodam-content-1">
        <Variable name="pemisah1.background.color" description="Background Color" type="color" default="#ffffff" value="#FCE8B2"/>
        <Variable name="pemisah1.text.color" description="Text Color" type="color" default="#444444"  value="#000000"/>
        </Group>

        <!-- ################### -->
        <!-- FEATURES -->
        <!-- ################### -->
        <Group description="Features" selector=".aroodam-content-2">
        <Variable name="features.background.color" description="Background Color" type="color" default="#ffffff" value="#ffffff"/>
        <Variable name="features.text.color" description="Title Color" type="color" default="#444444"  value="#535353"/>
        </Group>

        <!-- ################### -->
        <!-- PEMISAH 2 -->
        <!-- ################### -->
        <Group description="Pemisah 2" selector=".aroodam-content-3">
        <Variable name="pemisah2.background.color" description="Background Color" type="color" default="#ffffff" value="#003cc6"/>
        <Variable name="pemisah2.text.color" description="Text Color" type="color" default="#444444"  value="#FFFFFF"/>
        </Group>

        <!-- ################### -->
        <!-- TESTIMONI -->
        <!-- ################### -->
        <Group description="Testimoni" selector=".aroodam-content-4">
        <Variable name="testimoni.background.color" description="Background Color" type="color" default="#ffffff" value="#ffffff"/>
        <Variable name="testimoni.text.color" description="Title Color" type="color" default="#444444"  value="#535353"/>
        </Group>

        <!-- ################### -->
        <!-- PEMISAH 3 -->
        <!-- ################### -->
        <Group description="Pemisah 3" selector=".aroodam-content-5">
        <Variable name="pemisah3.background.color" description="Background Color" type="color" default="#ffffff" value="#ffffff"/>
        <Variable name="pemisah3.text.color" description="Text Color" type="color" default="#444444"  value="#535353"/>
        </Group>

        <!-- ################### -->
        <!-- CALL TO ACTION -->
        <!-- ################### -->
        <Group description="Call To Action" selector=".aroodam-content-6">
        <Variable name="cta.background.color" description="Background Color" type="color" default="#ffffff" value="#ffffff"/>
        <Variable name="cta.text.color" description="Title Color" type="color" default="#444444"  value="#535353"/>
        </Group>

        <!-- ################### -->
        <!-- PEMISAH 4 -->
        <!-- ################### -->
        <Group description="Pemisah 4" selector=".aroodam-content-7">
        <Variable name="pemisah4.background.color" description="Background Color" type="color" default="#ffffff" value="#ffffff"/>
        <Variable name="pemisah4.text.color" description="Text Color" type="color" default="#444444"  value="#535353"/>
        </Group>

        <!-- ################### -->
        <!-- FOOTER -->
        <!-- ################### -->
        <Group description="Footer" selector=".aroodam-content-8">
        <Variable name="footer.background.color" description="Background Color" type="color" default="#ffffff" value="#FCE8B2"/>
        <Variable name="footer.text.color" description="Title Color" type="color" default="#444444"  value="#000000"/>
        </Group>

        <!-- ################### -->
        <!-- FOOTER GLOBAL-->
        <!-- ################### -->
        <Group description="Footer Global" selector=".footer-global">
        <Variable name="footerglobal.background.color" description="Background Color" type="color" default="#ffffff" value="#ffffff"/>
        <Variable name="footerglobaltitle.text.color" description="Title Color" type="color" default="#444444"  value="#535353"/>
        <Variable name="footerglobal.text.color" description="Text Color" type="color" default="#444444"  value="#535353"/>
        </Group>

        <Group description="Post Title" selector="h2.post-title">
        <Variable name="post.title.font" description="Font" type="font"
        default="bold normal 48px Roboto, Arial, Tahoma, Helvetica, FreeSans, sans-serif" value="bold normal 48px Roboto, Arial, Tahoma, Helvetica, FreeSans, sans-serif"/>
        </Group>
        <Group description="Date Header" selector=".date-header">
        <Variable name="date.header.color" description="Text Color" type="color"
        default="$(body.text.color)" value="#222222"/>
        <Variable name="date.header.background.color" description="Background Color" type="color"
        default="transparent" value="rgba(64,64,64,0)"/>
        <Variable name="date.header.font" description="Text Font" type="font"
        default="normal bold 11px Roboto, Arial, Tahoma, Helvetica, FreeSans, sans-serif" value="normal bold 11px Roboto, Arial, Tahoma, Helvetica, FreeSans, sans-serif"/>
        <Variable name="date.header.padding" description="Date Header Padding" type="string" default="inherit" value="inherit"/>
        <Variable name="date.header.letterspacing" description="Date Header Letter Spacing" type="string" default="inherit" value="inherit"/>
        <Variable name="date.header.margin" description="Date Header Margin" type="string" default="inherit" value="inherit"/>
        </Group>
        <Group description="Post Footer" selector=".post-footer">
        <Variable name="post.footer.text.color" description="Text Color" type="color" default="#666666" value="#6e6e6e"/>
        <Variable name="post.footer.background.color" description="Background Color" type="color"
        default="#ffffff" value="#ffffff"/>
        <Variable name="post.footer.border.color" description="Shadow Color" type="color" default="#ffffff" value="#ffffff"/>
        </Group>
        <Group description="Gadgets" selector=".sidebar h3">
        <Variable name="widget.title.font" description="Title Font" type="font"
        default="normal bold 14px Roboto, Arial, Tahoma, Helvetica, FreeSans, sans-serif" value="normal bold 14px Roboto, Arial, Tahoma, Helvetica, FreeSans, sans-serif"/>
        <Variable name="widget.title.text.color" description="Title Color" type="color" default="#000000" value="#000000"/>
        <Variable name="widget.alternate.text.color" description="Alternate Color" type="color" default="#999999" value="#9d9d9d"/>
        </Group>
        <Group description="Images" selector=".main-inner">
        <Variable name="image.background.color" description="Background Color" type="color" default="#ffffff" value="#ffffff"/>
        <Variable name="image.border.color" description="Border Color" type="color" default="#eeeeee" value="#f0f0f0"/>
        <Variable name="image.text.color" description="Caption Text Color" type="color" default="$(body.text.color)" value="#222222"/>
        </Group>
        <Group description="Accents" selector=".content-inner">
        <Variable name="body.rule.color" description="Separator Line Color" type="color" default="#ffffff" value="#ffffff"/>
        <Variable name="tabs.border.color" description="Tabs Border Color" type="color" default="$(body.rule.color)" value="#ffffff"/>
        </Group>
        <Variable name="body.background" description="Body Background" type="background"
        color="$(body.background.color)" default="$(color) none repeat scroll top left" value="#adbbd5 url(https://themes.googleusercontent.com/image?id=1yCqzoXfTY3VhaTtS_2w31Trgk3LHk1kH1lSKIEivmW1OcaCeDlaGs_mBlO1T6KetEvus) no-repeat fixed top center /* Credit: mariusFM77 (http://www.istockphoto.com/portfolio/mariusFM77?platform=blogger) */"/>
        <Variable name="body.background.override" description="Body Background Override" type="string" default="" value=""/>
        <Variable name="body.background.gradient.cap" description="Body Gradient Cap" type="url"
        default="url(https://resources.blogblog.com/blogblog/data/1kt/simple/gradients_light.png)" value="none"/>
        <Variable name="body.background.gradient.tile" description="Body Gradient Tile" type="url"
        default="url(https://resources.blogblog.com/blogblog/data/1kt/simple/body_gradient_tile_light.png)" value="none"/>
        <Variable name="content.background.color.selector" description="Content Background Color Selector" type="string" default=".content-inner" value=".content-inner"/>
        <Variable name="content.padding" description="Content Padding" type="length" default="10px" min="0" max="100px" value="10px"/>
        <Variable name="content.padding.horizontal" description="Content Horizontal Padding" type="length" default="$(content.padding)" min="0" max="100px" value="10px"/>
        <Variable name="content.shadow.spread" description="Content Shadow Spread" type="length" default="40px" min="0" max="100px" value="40px"/>
        <Variable name="content.shadow.spread.webkit" description="Content Shadow Spread (WebKit)" type="length" default="5px" min="0" max="100px" value="5px"/>
        <Variable name="content.shadow.spread.ie" description="Content Shadow Spread (IE)" type="length" default="10px" min="0" max="100px" value="10px"/>
        <Variable name="main.border.width" description="Main Border Width" type="length" default="0" min="0" max="10px" value="0"/>
        <Variable name="header.background.gradient" description="Header Gradient" type="url" default="none" value="none"/>
        <Variable name="header.shadow.offset.left" description="Header Shadow Offset Left" type="length" default="-1px" min="-50px" max="50px" value="-1px"/>
        <Variable name="header.shadow.offset.top" description="Header Shadow Offset Top" type="length" default="-1px" min="-50px" max="50px" value="-1px"/>
        <Variable name="header.shadow.spread" description="Header Shadow Spread" type="length" default="1px" min="0" max="100px" value="1px"/>
        <Variable name="header.padding" description="Header Padding" type="length" default="30px" min="0" max="100px" value="30px"/>
        <Variable name="header.border.size" description="Header Border Size" type="length" default="1px" min="0" max="10px" value="1px"/>
        <Variable name="header.bottom.border.size" description="Header Bottom Border Size" type="length" default="$(header.border.size)" min="0" max="10px" value="1px"/>
        <Variable name="header.border.horizontalsize" description="Header Horizontal Border Size" type="length" default="0" min="0" max="10px" value="0"/>
        <Variable name="description.text.size" description="Description Text Size" type="string" default="140%" value="140%"/>



        <Variable name="tabs.margin.top" description="Tabs Margin Top" type="length" default="0" min="0" max="100px" value="0"/>
        <Variable name="tabs.margin.side" description="Tabs Side Margin" type="length" default="15px" min="0" max="100px" value="15px"/>
        <Variable name="tabs.background.gradient" description="Tabs Background Gradient" type="url"
        default="url(https://resources.blogblog.com/blogblog/data/1kt/simple/gradients_light.png)" value="url(https://resources.blogblog.com/blogblog/data/1kt/simple/gradients_light.png)"/>
        <Variable name="tabs.border.width" description="Tabs Border Width" type="length" default="1px" min="0" max="10px" value="1px"/>
        <Variable name="tabs.bevel.border.width" description="Tabs Bevel Border Width" type="length" default="1px" min="0" max="10px" value="1px"/>
        <Variable name="post.margin.bottom" description="Post Bottom Margin" type="length" default="25px" min="0" max="100px" value="25px"/>
        <Variable name="image.border.small.size" description="Image Border Small Size" type="length" default="2px" min="0" max="10px" value="2px"/>
        <Variable name="image.border.large.size" description="Image Border Large Size" type="length" default="5px" min="0" max="10px" value="5px"/>
        <Variable name="page.width.selector" description="Page Width Selector" type="string" default=".region-inner" value=".region-inner"/>
        <Variable name="page.width" description="Page Width" type="string" default="auto" value="auto"/>
        <Variable name="main.section.margin" description="Main Section Margin" type="length" default="15px" min="0" max="100px" value="15px"/>
        <Variable name="main.padding" description="Main Padding" type="length" default="15px" min="0" max="100px" value="15px"/>
        <Variable name="main.padding.top" description="Main Padding Top" type="length" default="30px" min="0" max="100px" value="30px"/>
        <Variable name="main.padding.bottom" description="Main Padding Bottom" type="length" default="30px" min="0" max="100px" value="30px"/>
        <Variable name="paging.background"
        color="$(content.background.color)"
        description="Background of blog paging area" type="background"
        default="transparent none no-repeat scroll top center" value="transparent none no-repeat scroll top center"/>
        <Variable name="footer.bevel" description="Bevel border length of footer" type="length" default="0" min="0" max="10px" value="0"/>
        <Variable name="mobile.background.overlay" description="Mobile Background Overlay" type="string"
        default="transparent none repeat scroll top left" value="transparent none repeat scroll top left"/>
        <Variable name="mobile.background.size" description="Mobile Background Size" type="string" default="auto" value="auto"/>
        <Variable name="mobile.button.color" description="Mobile Button Color" type="color" default="#ffffff"  value="#ffffff"/>
        <Variable name="startSide" description="Side where text starts in blog language" type="automatic" default="left"/>
        <Variable name="endSide" description="Side where text ends in blog language" type="automatic" default="right"/>
        */



/* CSS BUNDLE */
body{margin:0;padding:0 0 1px}.content-outer,.header-outer,.tabs-outer,.main-outer,.main-inner,.footer-outer,.post,.comments,.widget,.date-header,.inline-ad{position:relative;min-height:0;_position:static;_height:1%}.footer-outer{margin-bottom:-1px}.content-inner{padding:10px}.tabs-inner{padding:0 15px}.main-inner{padding:30px 0}.main-inner .column-center-inner,.main-inner .column-left-inner,.main-inner .column-right-inner{padding:0px}.footer-inner{padding:30px 15px}.section{margin:0 15px}.widget{margin:30px 0;_margin:0 0 10px}.section:first-child .widget:first-child{margin-top:0}.section:first-child #uds-searchControl+.widget{margin-top:0}.section:last-child .widget:last-child{margin-bottom:0}.tabs:first-child .widget{margin-bottom:0}body .navbar{height:30px;padding:0;margin:0}body .navbar .Navbar{position:absolute;z-index:10;left:0;width:100%;margin:0;padding:0;background:none;border:none}.header-inner .section{margin:0}.header-inner .widget{margin-left:30px;margin-right:30px}.header-inner .Header{margin:0}.header-inner .Header #header-inner{overflow:hidden}.header-inner .Header .titlewrapper{padding:22px 30px 0}.header-inner .Header .descriptionwrapper{padding:0 30px;margin-bottom:25px}.Header h1{margin-bottom:10px}.Header .description{margin:.5em 0 10px;padding:0 2px}a img{border:none;position:relative}h1,h2,h3,h4{margin:0;position:relative}h1 a:hover{text-decoration:none}h3 a:hover{text-decoration:none}.tabs .widget h2{display:none}.tabs .widget ul,.tabs .widget ul{margin:0;padding:0;overflow:hidden;list-style:none}.tabs .widget li,.tabs .widget li{margin:0;padding:0;float:left}.tabs .widget li a:hover{text-decoration:none}.widget{line-height:1.4}.widget ul{padding:0 0 0 1.25em;margin:0;line-height:1.2}.BlogList ul{padding:0}.BlogList li .blog-content{position:relative}.widget li,.BlogArchive #ArchiveList ul.flat li{padding:.25em 0;margin:0;text-indent:0}.widget .post-body ul, .widget .post-body ol{padding:0 2.5em;margin:.5em 0;line-height:1.4}.widget .post-body li{margin-bottom:.25em;padding-top:0;padding-bottom:0}.item-control{display:none}.item-control a,.item-action a{text-decoration:none !important}.widget-item-control{float:right;height:20px;margin-top:-20px;position:relative;z-index:10}.widget-item-control a{opacity:.5}.widget-item-control a:hover{opacity:1}.widget .widget-item-control a img{border:none;padding:none;background:none;-moz-box-shadow:none;-webkit-box-shadow:none;-ie-box-shadow:none;box-shadow:none}.post-body{width:100%;_overflow:hidden}.post-header,.post-footer{line-height:1.6}.post-footer-line>*{margin-right:1em}.post-footer-line>*:last-child{margin-right:0}.post-timestamp{margin-left:-1em}.post-footer-line>*:first-child{margin-left:0}.post .tr-caption-container{position:relative}.inline-ad{margin:2em 0;text-align:center;line-height:0}#comments .comment-author{padding-left:25px}.comment-body{margin:.5em 25px}.comment-footer{margin:.5em 25px 1.5em}.comment-body p{margin:0}#comments .avatar-comment-indent .comment-author{margin-left:-45px;padding-left:45px}.deleted-comment{font-style:italic;opacity:.5}.Profile img{margin:0 .75em .5em 0}.Profile .profile-datablock{margin:0 0 .5em}dt{font-weight:bold}table.section-columns td.first.columns-cell{border-left:none}.post-summary{padding-top:8px}#layout .header-outer,#layout .tabs-outer,#layout .main-outer,#layout .footer-outer{margin:5px 0 !important;}#layout .cap-top,#layout .cap-bottom{display:none}#layout .region-inner{padding:0 10px;margin:0}#layout .main-inner .column-center-inner,#layout .main-inner .column-left-inner,#layout .main-inner .column-right-inner{padding:0 5px}html{height:100%}body{min-height:100%;_height:100%;position:relative}.content{position:relative;word-wrap:break-word}.content-outer,.region-inner{min-height:0;margin:0 auto}.columns{zoom:1}.loading .columns{overflow:hidden}.columns-inner{_height:1%;min-height:0}.column-center-outer,.column-left-outer,.column-right-outer{position:relative;float:left;_display:inline;_overflow:hidden}.column-center-outer{width:100%}.column-left-outer{margin-left:-100%}.fauxcolumns{position:relative;_height:1%}.fauxcolumn-outer{position:absolute;top:0;bottom:0;height:expression(this.parentNode.offsetHeight + 'px');overflow:hidden}.fauxcolumn-outer .fauxborder-left,.fauxcolumn-outer .fauxborder-right,.fauxcolumn-inner{height:100%}.fauxcolumn-left-outer{left:0}.fauxcolumn-right-outer{right:0}.cap-top,.cap-bottom{position:relative;height:0;background-repeat:repeat-x}.cap-top .cap-left,.cap-top .cap-right,.cap-bottom .cap-left,.cap-bottom .cap-right{height:100%;background-repeat:no-repeat}.cap-top,.cap-top .cap-left{background-position:top left}.cap-bottom,.cap-bottom .cap-left{background-position:bottom left}.cap-top .cap-left,.cap-bottom .cap-left{float:left}.cap-top .cap-right{background-position:top right;float:right}.cap-bottom .cap-right{background-position:bottom right;float:right}.fauxborder-left{background-position:top left;background-repeat:repeat-y;position:relative;_height:1%}.fauxborder-right{background-position:top right;background-repeat:repeat-y;position:absolute;right:0;height:100%;_height:expression(this.parentNode.offsetHeight + 'px')}table.section-columns{border:none;table-layout:fixed;width:100%;position:relative}table.columns-2 td.columns-cell{width:50%}table.columns-3 td.columns-cell{width:33.33%}table.columns-4 td.columns-cell{width:25%}table.section-columns td.columns-cell{vertical-align:top}.body-fauxcolumns,.content-fauxcolumns{position:absolute;top:0;left:0;z-index:-1;height:100%;_height:expression(this.parentNode.offsetHeight + 'px');width:100%;overflow:hidden}.body-fauxcolumns .fauxcolumn-outer{width:100%}.content-fauxcolumns .fauxcolumn-outer{position:relative;overflow:visible;height:100%;margin:0 auto}.content-fauxcolumns .fauxcolumn-left{width:100%}section,nav,article,aside,hgroup,header,footer{display:block}time,mark{display:inline}.blog-list-container ul{padding-left:0}.blog-list-container ul li{padding-left:0;list-style:none;list-style-image:none;clear:left}.blog-list-container a{text-decoration:none}.blog-list-container a:hover{text-decoration:underline}.blog-list-container .blog-content{float:left;margin:0 0 5px 5px;text-indent:0;width:85%}.blog-list-container .blog-title{font-weight:bold;line-height:16px;margin:2px 0 0 0}.blog-list-container .blog-icon{float:left;margin-top:2px;vertical-align:top;text-indent:0;width:16px}.blog-list-container .item-content{font-size:95%;line-height:1.3em}.blog-list-container .item-thumbnail{float:left;margin:2px 5px 5px 0}.blog-list-container .item-time{font-size:95%;font-style:italic;clear:left}.blog-list-title{font-weight:bold}.blog-list-container .show-option{font-size:75%;text-align:right}.contact-form-widget{height:320;margin-left:0;max-width:250px;padding:0;padding-top:0;width:100%}.contact-form-success-message{background:#f9edbe;border:0 solid #f0c36d;bottom:0;box-shadow:0 2px 4px rgba(0,0,0,.2);color:#222;font-size:11px;line-height:19px;margin-left:0;opacity:1;position:static;text-align:center}.contact-form-error-message{background:#f9edbe;border:0 solid #f0c36d;bottom:0;box-shadow:0 2px 4px rgba(0,0,0,.2);color:#666;font-size:11px;font-weight:bold;line-height:19px;margin-left:0;opacity:1;position:static;text-align:center}.contact-form-success-message-with-border{background:#f9edbe;border:1px solid #f0c36d;bottom:0;box-shadow:0 2px 4px rgba(0,0,0,.2);color:#222;font-size:11px;line-height:19px;margin-left:0;opacity:1;position:static;text-align:center}.contact-form-error-message-with-border{background:#f9edbe;border:1px solid #f0c36d;bottom:0;box-shadow:0 2px 4px rgba(0,0,0,.2);color:#666;font-size:11px;font-weight:bold;line-height:19px;margin-left:0;opacity:1;position:static;text-align:center}.contact-form-cross{height:11px;margin:0 5px;vertical-align:-8.5%;width:11px}.contact-form-email,.contact-form-name{background:#fff;background-color:#fff;border:1px solid #d9d9d9;border-top:1px solid #c0c0c0;box-sizing:border-box;color:#333;display:inline-block;font-family:Arial,sans-serif;font-size:13px;height:24px;margin:0;margin-top:5px;padding:0;vertical-align:top}.contact-form-email-message{background:#fff;background-color:#fff;border:1px solid #d9d9d9;border-top:1px solid #c0c0c0;box-sizing:border-box;color:#333;display:inline-block;font-family:Arial,sans-serif;font-size:13px;margin:0;margin-top:5px;padding:0;vertical-align:top}.contact-form-email:hover,.contact-form-name:hover,.contact-form-email-message:hover{border:1px solid #b9b9b9;border-top:1px solid #a0a0a0;box-shadow:inset 0 1px 2px rgba(0,0,0,.1)}.contact-form-email:focus,.contact-form-name:focus,.contact-form-email-message:focus{border:1px solid #4d90fe;box-shadow:inset 0 1px 2px rgba(0,0,0,.3);outline:none}.contact-form-name,.contact-form-email,.contact-form-email-message{max-width:220px;width:100%}.contact-form-button{-webkit-border-radius:2px;-moz-border-radius:2px;-webkit-transition:all .218s;-moz-transition:all .218s;-o-transition:all .218s;-webkit-user-select:none;-moz-user-select:none;background-color:#f5f5f5;background-image:-webkit-gradient(linear,left top,left bottom,from(#f5f5f5),to(#f1f1f1));background-image:-webkit-linear-gradient(top,#f5f5f5,#f1f1f1);background-image:-moz-linear-gradient(top,#f5f5f5,#f1f1f1);background-image:-ms-linear-gradient(top,#f5f5f5,#f1f1f1);background-image:-o-linear-gradient(top,#f5f5f5,#f1f1f1);background-image:linear-gradient(top,#f5f5f5,#f1f1f1);border:1px solid #dcdcdc;border:1px solid rgba(0,0,0,.1);border-radius:2px;color:#444;cursor:default;display:inline-block;filter:progid:DXImageTransform.Microsoft.gradient(startColorStr='#f5f5f5',EndColorStr='#f1f1f1');font-family:"Arial","Helvetica",sans-serif;font-size:11px;font-weight:bold;height:24px;line-height:24px;margin-left:0;min-width:54px;*min-width:70px;padding:0 8px;text-align:center;transition:all .218s}.contact-form-button:hover,.contact-form-button.hover{-moz-box-shadow:0 1px 1px rgba(0,0,0,.1);-moz-transition:all 0;-o-transition:all 0;-webkit-box-shadow:0 1px 1px rgba(0,0,0,.1);-webkit-transition:all 0;background-color:#f8f8f8;background-image:-webkit-gradient(linear,left top,left bottom,from(#f8f8f8),to(#f1f1f1));background-image:-webkit-linear-gradient(top,#f8f8f8,#f1f1f1);background-image:-moz-linear-gradient(top,#f8f8f8,#f1f1f1);background-image:-ms-linear-gradient(top,#f8f8f8,#f1f1f1);background-image:-o-linear-gradient(top,#f8f8f8,#f1f1f1);background-image:linear-gradient(top,#f8f8f8,#f1f1f1);border:1px solid #c6c6c6;box-shadow:0 1px 1px rgba(0,0,0,.1);color:#222;filter:progid:DXImageTransform.Microsoft.gradient(startColorStr='#f8f8f8',EndColorStr='#f1f1f1');transition:all 0}.contact-form-button.focus,.contact-form-button.right.focus,.contact-form-button.mid.focus,.contact-form-button.left.focus{border:1px solid #4d90fe;outline:none;z-index:4 !important}.contact-form-button-submit:focus,.contact-form-button-submit.focus{-moz-box-shadow:inset 0 0 0 1px rgba(255,255,255,.5);-webkit-box-shadow:inset 0 0 0 1px rgba(255,255,255,.5);box-shadow:inset 0 0 0 1px rgba(255,255,255,.5)}.contact-form-button-submit:focus,.contact-form-button-submit.focus{border-color:#404040}.contact-form-button-submit:focus:hover,.contact-form-button-submit.focus:hover{-moz-box-shadow:inset 0 0 0 1px #fff,0 1px 1px rgba(0,0,0,.1);-webkit-box-shadow:inset 0 0 0 1px #fff,0 1px 1px rgba(0,0,0,.1);box-shadow:inset 0 0 0 1px #fff,0 1px 1px rgba(0,0,0,.1)}.contact-form-button-submit{background-color:#666;background-image:-webkit-gradient(linear,left top,left bottom,from(#777),to(#555));background-image:-webkit-linear-gradient(top,#777,#555);background-image:-moz-linear-gradient(top,#777,#555);background-image:-ms-linear-gradient(top,#777,#555);background-image:-o-linear-gradient(top,#777,#555);background-image:linear-gradient(top,#777,#555);border:1px solid #505050;color:#fff;filter:progid:DXImageTransform.Microsoft.gradient(startColorStr='#777777',EndColorStr='#555555')}.contact-form-button-submit:hover{background-color:#555;background-image:-webkit-gradient(linear,left top,left bottom,from(#666),to(#444));background-image:-webkit-linear-gradient(top,#666,#444);background-image:-moz-linear-gradient(top,#666,#444);background-image:-ms-linear-gradient(top,#666,#444);background-image:-o-linear-gradient(top,#666,#444);background-image:linear-gradient(top,#666,#444);border:1px solid #404040;color:#fff;filter:progid:DXImageTransform.Microsoft.gradient(startColorStr='#666666',EndColorStr='#444444')}.contact-form-button-submit:active,.contact-form-button-submit:focus:active,.contact-form-button-submit.focus:active{-webkit-box-shadow:inset 0 1px 2px rgba(0,0,0,.3);-moz-box-shadow:inset 0 1px 2px rgba(0,0,0,.3);box-shadow:inset 0 1px 2px rgba(0,0,0,.3)}.contact-form-button-submit{background-color:#4d90fe;background-image:-webkit-gradient(linear,left top,left bottom,from(#4d90fe),to(#4787ed));background-image:-webkit-linear-gradient(top,#4d90fe,#4787ed);background-image:-moz-linear-gradient(top,#4d90fe,#4787ed);background-image:-ms-linear-gradient(top,#4d90fe,#4787ed);background-image:-o-linear-gradient(top,#4d90fe,#4787ed);background-image:linear-gradient(top,#4d90fe,#4787ed);border-color:#3079ed;filter:progid:DXImageTransform.Microsoft.gradient(startColorStr='#4d90fe',EndColorStr='#4787ed')}.contact-form-button-submit:hover{background-color:#357ae8;background-image:-webkit-gradient(linear,left top,left bottom,from(#4d90fe),to(#357ae8));background-image:-webkit-linear-gradient(top,#4d90fe,#357ae8);background-image:-moz-linear-gradient(top,#4d90fe,#357ae8);background-image:-ms-linear-gradient(top,#4d90fe,#357ae8);background-image:-o-linear-gradient(top,#4d90fe,#357ae8);background-image:linear-gradient(top,#4d90fe,#357ae8);border-color:#2f5bb7;filter:progid:DXImageTransform.Microsoft.gradient(startColorStr='#4d90fe',EndColorStr='#357ae8')}.contact-form-button.disabled,.contact-form-button.disabled:hover,.contact-form-button.disabled:active{background:none;border:1px solid #f3f3f3;border:1px solid rgba(0,0,0,.05);color:#b8b8b8;cursor:default;pointer-events:none}.contact-form-button-submit.disabled,.contact-form-button-submit.disabled:hover,.contact-form-button-submit.disabled:active{-ms-filter:"progid:DXImageTransform.Microsoft.Alpha(Opacity=50)";background-color:#666;border:1px solid #505050;color:#fff;filter:alpha(opacity=50);opacity:.5}.contact-form-button-submit.disabled,.contact-form-button-submit.disabled:hover,.contact-form-button-submit.disabled:active{background-color:#4d90fe;border-color:#3079ed}.Example{}.FollowByEmail .follow-by-email-inner{position:relative}.FollowByEmail .follow-by-email-inner span{display:block;position:relative;margin-right:74px}.FollowByEmail .follow-by-email-inner input{font-family:arial,sans-serif}.FollowByEmail .follow-by-email-inner::-webkit-input-placeholder,.FollowByEmail .follow-by-email-inner input:-moz-placeholder{font-size:13px;font-family:arial,sans-serif;color:#999}.FollowByEmail .follow-by-email-inner .follow-by-email-address{width:100%;height:22px;font-size:13px;border:1px inset}.FollowByEmail .follow-by-email-inner .follow-by-email-submit{width:60px;margin:0;margin-left:8px;border:0;border-radius:2px;-moz-border-radius:2px;background:#000 ;background:rgba(0,0,0,.6);color:#fff;cursor:pointer;font-size:13px;height:26px;z-index:0}.FollowByEmail .widget-item-control{margin-top:5px}a.follower-link{cursor:pointer}a.next-page-link{cursor:pointer}.follower{width:32px;height:32px;float:left;margin:2px}.follower img{width:32px;clip:rect(0,32px,32px,0);position:absolute}div.clear{clear:both}.label-size-1{font-size:80%;filter:alpha(80);opacity:.8}.label-size-2{font-size:90%;filter:alpha(90);opacity:.9}.label-size-3{font-size:100%}.label-size-4{font-size:120%}.label-size-5{font-size:160%}.cloud-label-widget-content{text-align:justify}.label-count{white-space:nowrap}.label-size{line-height:1.2}.quickedit{cursor:pointer}.Navbar iframe{display:block}#navbar-iframe{display:block;height:30px}.crosscol .PageList UL,.footer .PageList UL{list-style:none;margin:0;padding:0}.crosscol .PageList LI,.footer .PageList LI{list-style:none;float:left;padding-right:.75em;margin:.75em;background:none}.crosscol .PageList H2{display:none}.PageList LI A{font-weight:normal}.PageList LI.selected A{font-weight:bold;text-decoration:none}.PlusBadge{}.PlusFollowers{}.PlusOne{}.PopularPosts .item-thumbnail{float:left;margin:0 5px 5px 0}.PopularPosts .widget-content ul li{padding:.7em 0}.PopularPosts img{padding-right:.4em}.PopularPosts .item-title{padding-bottom:.2em}.default-avatar{display:none}.profile-img{float:left;margin:0 5px 5px}.profile-data{margin:0}.profile-datablock{margin:.5em 0}.profile-name-link{background:no-repeat left top;box-sizing:border-box;display:inline-block;max-width:100%;min-height:20px;padding-left:20px}.profile-textblock{margin:.5em 0}body{overflow-wrap:break-word;word-break:break-word;word-wrap:break-word}.hidden{display:none}.invisible{visibility:hidden}.container::after,.float-container::after{clear:both;content:'';display:table}.clearboth{clear:both}.dim-overlay{background-color:rgba(0,0,0,.54);height:100vh;left:0;position:fixed;top:0;width:100%}#sharing-dim-overlay{background-color:transparent}input::-ms-clear{display:none}.blogger-logo,.svg-icon-24.blogger-logo{fill:#ff9800;opacity:1}.widget.Sharing .sharing-button{display:none}.widget.Sharing .sharing-buttons li{padding:0}.widget.Sharing .sharing-buttons li span{display:none}.post-share-buttons{position:relative}.share-buttons .svg-icon-24,.centered-bottom .share-buttons .svg-icon-24{fill:#000}.sharing-open.touch-icon-button:focus .touch-icon,.sharing-open.touch-icon-button:active .touch-icon{background-color:transparent}.share-buttons{background-color:#fff;border-radius:2px;box-shadow:0 2px 2px 0 rgba(0,0,0,.14),0 3px 1px -2px rgba(0,0,0,.2),0 1px 5px 0 rgba(0,0,0,.12);color:#000;list-style:none;margin:0;padding:8px 0;position:absolute;top:-11px;min-width:200px;z-index:101}.share-buttons.hidden{display:none}.sharing-button{background:transparent;border:0;margin:0;outline:none;padding:0;cursor:pointer}.share-buttons li{margin:0;height:48px}.share-buttons li:last-child{margin-bottom:0}.share-buttons li .sharing-platform-button{box-sizing:border-box;cursor:pointer;display:block;height:100%;margin-bottom:0;padding:0 16px;position:relative;width:100%}.share-buttons li .sharing-platform-button:focus,.share-buttons li .sharing-platform-button:hover{background-color:rgba(128,128,128,.1);outline:none}.share-buttons li svg[class^="sharing-"],.share-buttons li svg[class*=" sharing-"]{position:absolute;top:10px}.share-buttons li span.sharing-platform-button,.share-buttons li span.sharing-platform-button{position:relative;top:0}.share-buttons li .platform-sharing-text{display:block;font-size:16px;line-height:48px;white-space:nowrap}.share-buttons li .platform-sharing-text{margin-$startSide:56px}{"version":3,"file":"sharing_css.css","sources":[ "../../../../../../../../../../../java/com/google/blogger/b2/layouts/widgets/sharing/sharing.scss","../../../../../../../../../../../java/com/google/blogger/b2/staticresources/layouts/skins/responsive/scss/_functions.scss","../../../../../../../../../../../java/com/google/blogger/b2/staticresources/layouts/skins/responsive/scss/_variables.scss","../../../../../../../../../../../java/com/google/blogger/b2/staticresources/layouts/skins/responsive/scss/common.scss","../../../../../../../../../../../java/com/google/blogger/b2/staticresources/layouts/skins/responsive/scss/sharing.scss" ],"names":[],"mappings":"AGAA,AAAA,IAAI,CAAC;EACH,aAAa,EAAE,UAAU;EACzB,UAAU,EAAE,UAAU;EACtB,SAAS,EAAE,UAAU;CACtB;;AAED,AAAA,OAAO,CAAC;EACN,OAAO,EAAE,IAAI;CACd;;AAED,AAAA,UAAU,CAAC;EACT,UAAU,EAAE,MAAM;CACnB;;AAQD,AAAA,UAAU,AAAA,OAAO;AACjB,AAAA,gBAAgB,AAAA,OAAO,CAAC;EANtB,KAAK,EAAE,IAAI;EACX,OAAO,EAAE,EAAE;EACX,OAAO,EAAE,KAAK;CAMf;;AAED,AAAA,UAAU,CAAC;EACT,KAAK,EAAE,IAAI;CACZ;;AAwFD,AAAA,YAAY,CAAC;EACX,gBAAgB,EAJJ,mBAAkB;EAK9B,MAAM,EAAE,KAAK;EACb,IAAI,EAAE,CAAC;EACP,QAAQ,EAAE,KAAK;EACf,GAAG,EAAE,CAAC;EACN,KAAK,EAAE,IAAI;CACZ;;AAED,AAAA,oBAAoB,CAAC;EACnB,gBAAgB,EAAE,WAAW;CAC9B;;AAYD,AAAA,KAAK,AAAA,WAAW,CAAC;EACf,OAAO,EAAE,IAAI;CACd;;AAED,AAAA,aAAa;AACb,AAAA,YAAY,AAAA,aAAa,CAAC;EACxB,IAAI,EDjHe,OAAO;ECkH1B,OAAO,EAAE,GAAG;CACb;;ACtID;;;GAGG;AAMH,6BAA6B;AAU7B,2BAA2B;AAC3B,AAAgB,OAAT,AAAA,QAAQ,CAAC,eAAe,CAAC;EAC9B,OAAO,EAAE,IAAI;CACd;;AAED,AAAiC,OAA1B,AAAA,QAAQ,CAAC,gBAAgB,CAAC,EAAE,CAAC;EAClC,OAAO,EAAE,CAAC;CACX;;AAED,AAAoC,OAA7B,AAAA,QAAQ,CAAC,gBAAgB,CAAC,EAAE,CAAC,IAAI,CAAC;EACvC,OAAO,EAAE,IAAI;CACd;;AAED,AAAA,mBAAmB,CAAC;EAClB,QAAQ,EAAE,QAAQ;CACnB;;AAED,AAAe,cAAD,CAAC,YAAY;AAC3B,AAAgC,gBAAhB,CAAC,cAAc,CAAC,YAAY,CAAC;EAC3C,IAAI,EAhCe,IAAI;CAiCxB;;AAED,AAAsC,aAAzB,AAAA,kBAAkB,AAAA,MAAM,CAAC,WAAW;AACjD,AAAuC,aAA1B,AAAA,kBAAkB,AAAA,OAAO,CAAC,WAAW,CAAC;EACjD,gBAAgB,EAAE,WAAW;CAC9B;;AAED,AAAA,cAAc,CAAC;EACb,gBAAgB,EA1CS,IAAI;EA2C7B,aAAa,EAAE,GAAG;EAClB,UAAU,EAAE,CAAC,CAAC,GAAG,CAAC,GAAG,CAAC,CAAC,CAAC,mBAAe,EAAE,CAAC,CAAC,GAAG,CAAC,GAAG,CAAE,IAAG,CAAC,kBAAc,EAAE,CAAC,CAAC,GAAG,CAAC,GAAG,CAAC,CAAC,CAAC,mBAAe;EACnG,KAAK,EA5Cc,IAAI;EA6CvB,UAAU,EAAE,IAAI;EAChB,MAAM,EAAE,CAAC;EACT,OAAO,EA3CwB,GAAG,CA2CO,CAAC;EAC1C,QAAQ,EAAE,QAAQ;EAClB,GAAG,EAtCkB,KAAI;EAuCzB,oEAAoE;EACpE,0EAA0E;EAC1E,SAAS,EA9Ce,KAAK;EA+C7B,OAAO,EJtEe,GAAG;CIuE1B;;AAED,AAAA,cAAc,AAAA,OAAO,CAAC;EACpB,OAAO,EAAE,IAAI;CACd;;AAED,AAAA,eAAe,CAAC;EDhCd,UAAU,EAAE,WAAW;EACvB,MAAM,EAAE,CAAC;EACT,MAAM,EAAE,CAAC;EACT,OAAO,EAAE,IAAI;EACb,OAAO,EAAE,CAAC;EC8BV,MAAM,EAAE,OAAO;CAChB;;AAED,AAAe,cAAD,CAAC,EAAE,CAAC;EAChB,MAAM,EAAE,CAAC;EACT,MAAM,EA5DoB,IAAI;CA6D/B;;AAED,AAAe,cAAD,CAAC,EAAE,AAAA,WAAW,CAAC;EAC3B,aAAa,EAAE,CAAC;CACjB;;AAED,AAAkB,cAAJ,CAAC,EAAE,CAAC,wBAAwB,CAAC;EACzC,UAAU,EAAE,UAAU;EACtB,MAAM,EAAE,OAAO;EACf,OAAO,EAAE,KAAK;EACd,MAAM,EAAE,IAAI;EACZ,aAAa,EAAE,CAAC;EAChB,OAAO,EAAE,CAAC,CA3EuB,IAAI;EA4ErC,QAAQ,EAAE,QAAQ;EAClB,KAAK,EAAE,IAAI;CACZ;;AAED,AAAkB,cAAJ,CAAC,EAAE,CAAC,wBAAwB,AAAA,MAAM;AAChD,AAAkB,cAAJ,CAAC,EAAE,CAAC,wBAAwB,AAAA,MAAM,CAAC;EAC/C,gBAAgB,EAAE,wBAAwB;EAC1C,OAAO,EAAE,IAAI;CACd;;AAED,AAAkB,cAAJ,CAAC,EAAE,CAAC,GAAG,CAAA,AAAA,KAAC,EAAO,UAAU,AAAjB;AACtB,AAAkB,cAAJ,CAAC,EAAE,CAAC,GAAG,CAAA,AAAA,KAAC,EAAO,WAAW,AAAlB,EAAoB;EACxC,QAAQ,EAAE,QAAQ;EAClB,GAAG,EAAE,IAAI;CACV;;AAED,qEAAqE;AACrE,AAAkB,cAAJ,CAAC,EAAE,CAAC,IAAI,AAAA,wBAAwB;AAC9C,AAAkB,cAAJ,CAAC,EAAE,CAAC,IAAI,AAAA,wBAAwB,CAAC;EAC7C,QAAQ,EAAE,QAAQ;EAClB,GAAG,EAAE,CAAC;CACP;;AAED,AAAkB,cAAJ,CAAC,EAAE,CAAC,sBAAsB,CAAC;EACvC,OAAO,EAAE,KAAK;EACd,SAAS,EAAE,IAAI;EACf,mEAAmE;EACnE,WAAW,EArGe,IAAI;EAsG9B,WAAW,EAAE,MAAM;CACpB;;AAED,AAAkB,cAAJ,CAAC,EAAE,CAAC,sBAAsB,CAAC;EACvC,iBAAoB,EAvGM,IAAuE;CAwGlG"}.Stats .counter-wrapper{display:inline-block;font-size:24px;font-weight:bold;height:30px;line-height:30px;vertical-align:top;direction:ltr}.Stats img{margin-right:10px;vertical-align:top}.Stats .graph-counter-wrapper{color:#fff}.Stats .digit{background:url("/img/widgets/stats-flipper.png") no-repeat left !important;border:1px solid #fff;display:inline-block;height:28px;line-height:28px;margin-left:-1px;position:relative;text-align:center;width:22px}.Stats .blind-plate{border-bottom:1px solid #fff;border-top:1px solid #000;filter:alpha(opacity=65);height:0;left:0;opacity:.65;position:absolute;top:13px;width:22px}.Stats .stage-0{background-position:0 0 !important}.Stats .stage-1{background-position:-22px 0 !important}.Stats .stage-2{background-position:-44px 0 !important}.Stats .stage-3{background-position:-66px 0 !important}.widget.Subscribe{position:static}.widget.Subscribe .widget-content{zoom:1}.subscribe-feed-title{float:left}.subscribe{cursor:pointer;color:#999}.subscribe a{color:#999}.subscribe-wrapper{margin:.5em;padding:0;position:relative;zoom:1}div.subscribe{cursor:pointer;margin:0;padding:0;text-align:left;width:144px}div.subscribe div.top{filter:progid:DXImageTransform.Microsoft.AlphaImageLoader(src='https://resources.blogblog.com/img/widgets/s_top.png',sizingMethod='crop');font-size:1em;padding:4px 0 1px;width:144px}html>body div.subscribe div.top{background:url(https://resources.blogblog.com/img/widgets/s_top.png) top left no-repeat}span.inner{margin:0;padding:0}div.subscribe div.top span.inner{margin:0 5px}.feed-icon{vertical-align:baseline;display:inline}div.subscribe div.bottom{filter:progid:DXImageTransform.Microsoft.AlphaImageLoader(src='https://resources.blogblog.com/img/widgets/s_bottom.png',sizingMethod='crop');font-size:3px;height:3px;line-height:0}.subscribe-wrapper .expanded{position:absolute;top:0;z-index:20}html>body div.subscribe div.bottom{background:url(https://resources.blogblog.com/img/widgets/s_bottom.png) bottom left no-repeat;margin-bottom:0;padding-bottom:0;width:144px}.feed-reader-links{list-style:none;margin:10px 20px;padding:0;position:relative}.subscribe-dropdown-arrow{float:right;margin-right:6px;margin-top:4px}.feed-reader-links{list-style:none;margin:0;padding:0}a.feed-reader-link{display:block;font-weight:normal;margin:.5em;text-decoration:none;z-index:1000}.feed-reader-link img{border:0;display:inline}.Translate a.goog-te-menu-value{text-decoration:none}.Translate .goog-te-menu-value span{color:#000}.Translate .goog-te-gadget a:link.goog-logo-link{font-size:12px;font-weight:bold;color:#444;text-decoration:none}.Translate .goog-te-combo{background-color:#f5f5f5;color:#444;border:1px solid #dcdcdc;padding:6px;font-family:Arial,Helvetica,sans-serif}.wikipedia-search-main-container{max-width:350px}.wikipedia-search-wiki-link{vertical-align:middle;width:8%}.wikipedia-search-input{border:1px solid #d9d9d9;border-top:1px solid #c0c0c0;-webkit-box-sizing:border-box;-moz-box-sizing:border-box;-ms-box-sizing:border-box;box-sizing:border-box;height:28px;padding-left:4px;vertical-align:top;width:60%}.wikipedia-search-input:hover{border:1px solid #b9b9b9;border-top:1px solid #a0a0a0;-webkit-box-shadow:inset 0 1px 2px rgba(0,0,0,.1);-moz-box-shadow:inset 0 1px 2px rgba(0,0,0,.1);-ms-box-shadow:inset 0 1px 2px rgba(0,0,0,.1);box-shadow:inset 0 1px 2px rgba(0,0,0,.1)}.wikipedia-search-input:focus{border:1px solid #4d90fe;-webkit-box-shadow:inset 0 1px 2px rgba(0,0,0,.3);-moz-box-shadow:inset 0 1px 2px rgba(0,0,0,.3);-ms-box-shadow:inset 0 1px 2px rgba(0,0,0,.3);box-shadow:inset 0 1px 2px rgba(0,0,0,.3);outline:none}.wikipedia-search-form{margin:0;overflow:hidden;padding-bottom:0;padding-left:6px}.wikipedia-search-results-header{border-bottom:1px solid #ebebeb;display:none;font-weight:bold;height:19px;padding-top:3px}.wikipedia-search-button{background-color:#4d90fe;background-image:url('/img/widgets/icon_wikipedia_search.png');background-position:center;background-repeat:no-repeat;border:1px solid #3079ed;-webkit-border-radius:2px;-moz-border-radius:2px;-ms-border-radius:2px;border-radius:2px;color:transparent;font-size:11px;font-weight:bold;height:28px;text-align:center;width:38px}.wikipedia-search-button:hover{background-color:#357ae8;border:1px solid #2f5bb7;color:transparent}.wikipedia-search-button:focus{-webkit-box-shadow:inset 0 0 0 1px #fff;-moz-box-shadow:inset 0 0 0 1px #fff;-ms-box-shadow:inset 0 0 0 1px #fff;box-shadow:inset 0 0 0 1px #fff}.wikipedia-search-results{color:#dd4b39;padding-top:2px}.wikipedia-search-result-link a:link,.wikipedia-search-more a:visited,.wikipedia-search-result-link a:visited{text-decoration:none}.wikipedia-search-more a:hover,.wikipedia-search-result-link a:hover,.wikipedia-search-more a:active,.wikipedia-search-result-link a:active{text-decoration:underline}.wikipedia-search-more a:link{text-decoration:none}.wikipedia-search-main-container{padding-top:5px}.wikipedia-searchtable{position:relative;right:6px}.wikipedia-search-bar{white-space:nowrap}.wikipedia-icon{padding-bottom:5px}.wikipedia-input-box{padding:0 2px}#ArchiveList .toggle{cursor:pointer;font-family:Arial,sans-serif}#ArchiveList .toggle-open{_font-size:1.7em;line-height:.6em}#ArchiveList{text-align:left}#ArchiveList a.post-count-link,#ArchiveList a.post-count-link:link,#ArchiveList a.post-count-link:visited{text-decoration:none}#ArchiveList a.toggle,#ArchiveList a.toggle:link,#ArchiveList a.toggle:visited,#ArchiveList a.toggle:hover{color:inherit;text-decoration:none}.BlogArchive #ArchiveList ul li{background:none;list-style:none;list-style-image:none;list-style-position:outside;border-width:0;padding-left:15px;text-indent:-15px;margin:.25em 0;background-image:none}.BlogArchive #ArchiveList ul ul li{padding-left:1.2em}.BlogArchive #ArchiveList ul{margin:0;padding:0;list-style:none;list-style-image:none;border-width:0}.BlogArchive #ArchiveList ul.posts li{padding-left:1.3em}#ArchiveList .collapsed ul{display:none}.post-footer abbr{border:none}.author-profile{margin:5px 5px 0 0;overflow:hidden}.author-profile img{border:1px solid #efefef;float:left;margin-right:5px}#blog-pager-newer-link{float:left}#blog-pager-older-link{float:right}#blog-pager{margin:1em 0;text-align:center;overflow:hidden}.backlink-toggle-zippy{padding-right:11px;margin-right:.1em;cursor:pointer;cursor:hand;background:url(https://resources.blogblog.com/img/triangle_ltr.gif) no-repeat left center}.expanded-backlink .backlink-toggle-zippy{background-image:url("https://resources.blogblog.com/img/triangle_open.gif")}.collapsed-backlink .collapseable{display:none}.status-msg-wrap{font-size:110%;width:90%;margin:10px auto;position:relative}.status-msg-border{border:1px solid #000;filter:alpha(opacity=40);-moz-opacity:.4;opacity:.4;width:100%;position:relative}.status-msg-bg{background-color:#ccc;opacity:.8;filter:alpha(opacity=30);-moz-opacity:.8;width:100%;position:relative;z-index:1}.status-msg-body{text-align:center;padding:.3em 0;width:100%;position:absolute;z-index:4}.status-msg-hidden{visibility:hidden;padding:.3em 0}.status-msg-wrap a{padding-left:.4em;text-decoration:underline}.reactions-label{margin:3px 0 0 0}.reactions-label-cell{line-height:2.3em}.reactions-iframe{background:transparent;height:2.3em;width:100%;border:0}#comment-actions{background:transparent;border:0;padding:0;position:absolute;height:25px}#comments .blogger-comment-icon,.blogger-comment-icon{line-height:16px;background:url(/img/b16-rounded.gif) left no-repeat;padding-left:20px}#comments .openid-comment-icon,.openid-comment-icon{line-height:16px;background:url(/img/openid16-rounded.gif) left no-repeat;padding-left:20px}#comments .anon-comment-icon,.anon-comment-icon{line-height:16px;background:url(/img/anon16-rounded.gif) left no-repeat;padding-left:20px}.comment-form{clear:both;_width:410px}.comment-link{white-space:nowrap}.paging-control-container{float:right;margin:0 6px 0 0;font-size:80%}.unneeded-paging-control{visibility:hidden}#comments-block .avatar-image-container img{-ms-interpolation-mode:bicubic;border:1px solid #ccc;float:right}#comments-block .avatar-image-container.avatar-stock img{border-width:0;padding:1px}#comments-block .avatar-image-container{height:37px;left:-45px;position:absolute;width:37px}#comments-block.avatar-comment-indent{margin-left:45px;position:relative}#comments-block.avatar-comment-indent dd{margin-left:0}iframe.avatar-hovercard-iframe{border:0 none;padding:0;width:25em;height:9.4em;margin:.5em}.comments{clear:both;margin-top:10px;margin-bottom:0}.comments .comments-content{margin-bottom:16px}.comments .comment .comment-actions a{padding-right:5px;padding-top:5px}.comments .comment .comment-actions a:hover{text-decoration:underline}.comments .comments-content .comment-thread ol{list-style-type:none;padding:0;text-align:left}.comments .comments-content .inline-thread{padding:.5em 1em}.comments .comments-content .comment-thread{margin:8px 0}.comments .comments-content .comment-thread:empty{display:none}.comments .comments-content .comment-replies{margin-left:36px;margin-top:1em}.comments .comments-content .comment{margin-bottom:16px;padding-bottom:8px}.comments .comments-content .comment:first-child{padding-top:16px}.comments .comments-content .comment:last-child{border-bottom:0;padding-bottom:0}.comments .comments-content .comment-body{position:relative}.comments .comments-content .user{font-style:normal;font-weight:bold}.comments .comments-content .icon.blog-author{display:inline-block;height:18px;margin:0 0 -4px 6px;width:18px}.comments .comments-content .datetime{margin-left:6px}.comments .comments-content .comment-header,.comments .comments-content .comment-content{margin:0 0 8px}.comments .comments-content .comment-content{text-align:justify}.comments .comments-content .owner-actions{position:absolute;right:0;top:0}.comments .comments-replybox{border:none;height:250px;width:100%}.comments .comment-replybox-single{margin-left:48px;margin-top:5px}.comments .comment-replybox-thread{margin-top:5px}.comments .comments-content .loadmore a{display:block;padding:10px 16px;text-align:center}.comments .thread-toggle{cursor:pointer;display:inline-block}.comments .continue{cursor:pointer}.comments .continue a{display:block;font-weight:bold;padding:.5em}.comments .comments-content .loadmore{cursor:pointer;margin-top:3em;max-height:3em}.comments .comments-content .loadmore.loaded{max-height:0;opacity:0;overflow:hidden}.comments .thread-chrome.thread-collapsed{display:none}.comments .thread-toggle{display:inline-block}.comments .thread-toggle .thread-arrow{display:inline-block;height:6px;margin:.3em;overflow:visible;padding-right:4px;width:7px}.comments .thread-expanded .thread-arrow{background:url("data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAcAAAAHCAYAAADEUlfTAAAAG0lEQVR42mNgwAfKy8v/48I4FeA0AacVDFQBAP9wJkE/KhUMAAAAAElFTkSuQmCC") no-repeat scroll 0 0 transparent}.comments .thread-collapsed .thread-arrow{background:url("data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAcAAAAHCAYAAADEUlfTAAAAJUlEQVR42mNgAILy8vL/DLgASBKnApgkVgXIkhgKiNKJ005s4gDLbCZBiSxfygAAAABJRU5ErkJggg==") no-repeat scroll 0 0 transparent}.comments .avatar-image-container{float:left;max-height:36px;overflow:hidden;width:36px}.comments .avatar-image-container img{max-width:36px}.comments .comment-block{margin-left:48px;position:relative}.comments .hidden{display:none}@media screen and (max-device-width:480px){.comments .comments-content .comment-replies{margin-left:0}}table.tr-caption-container{padding:4px;margin-bottom:.5em}td.tr-caption{font-size:80%}.icon-action{border-style:none !important;margin:0 0 0 .5em !important;vertical-align:middle}.comment-action-icon{width:13px;height:13px;margin-top:3px}.delete-comment-icon{background:url("/img/icon_delete13.gif") no-repeat left;padding:7px}#comment-popup{position:absolute;visibility:hidden;width:100px;height:20px}@media all{.BLOG_mobile_video_class{display:none}}@media handheld{.BLOG_mobile_video_class{display:inline}.BLOG_video_class{display:none}}.post-share-buttons{display:inline-block;margin-top:.5em;vertical-align:middle}.share-button{width:20px;height:20px;background:url(/img/share_buttons_20_3.png) no-repeat left !important;overflow:hidden;margin-left:-1px;position:relative}.dummy-container,.google-plus-share-container{vertical-align:top;padding-left:.3em}a:hover.share-button{text-decoration:none;z-index:1}.share-button-link-text{display:block;text-indent:-9999px}.sb-email{background-position:0 0 !important}a:hover.sb-email{background-position:0 -20px !important}a:active.sb-email{background-position:0 -40px !important}.sb-blog{background-position:-20px 0 !important}a:hover.sb-blog{background-position:-20px -20px !important}a:active.sb-blog{background-position:-20px -40px !important}.sb-twitter{background-position:-40px 0 !important}a:hover.sb-twitter{background-position:-40px -20px !important}a:active.sb-twitter{background-position:-40px -40px !important}.sb-facebook{background-position:-60px 0 !important}a:hover.sb-facebook{background-position:-60px -20px !important}a:active.sb-facebook{background-position:-60px -40px !important}.sb-buzz{display:none !important}.sb-pinterest{background-position:-100px 0 !important}a:hover.sb-pinterest{background-position:-100px -20px !important}a:active.sb-pinterest{background-position:-100px -40px !important}.sb-google{background:url(/img/plusone/plusonepreview.png) no-repeat;height:20px;vertical-align:top;width:82px}.goog-inline-block{position:relative;display:-moz-inline-box;display:inline-block}* html .goog-inline-block{display:inline}*:first-child+html .goog-inline-block{display:inline}.goog-custom-button{margin:2px;border:0;padding:0;font-family:Arial,sans-serif;color:#000;text-decoration:none;list-style:none;vertical-align:middle;cursor:default;outline:none}.goog-custom-button-outer-box,.goog-custom-button-inner-box{border-style:solid;border-color:transparent;vertical-align:top}.goog-custom-button-checked .goog-custom-button-outer-box,.goog-custom-button-checked .goog-custom-button-inner-box{border-color:#ccc}.goog-custom-button-outer-box{margin:0;border-width:1px 0;padding:0}.goog-custom-button-inner-box{-moz-box-orient:vertical;margin:0 -1px;border-width:0 1px;padding:3px 4px;white-space:nowrap}* html .goog-custom-button-inner-box{left:-1px}* html .goog-custom-button-rtl .goog-custom-button-outer-box{left:-1px}* html .goog-custom-button-rtl .goog-custom-button-inner-box{right:auto}*:first-child+html .goog-custom-button-inner-box{left:-1px}*:first-child+html .goog-custom-button-rtl .goog-custom-button-inner-box{left:1px}::root .goog-custom-button,::root .goog-custom-button-outer-box{line-height:0}::root .goog-custom-button-inner-box{line-height:normal}.goog-custom-button-active,.goog-custom-button-checked{background-color:#faf6bc;background-position:bottom left}.blog-mobile-link{padding:15px}#mobile-share-button{height:18px;padding:1px 10px;text-align:center;vertical-align:top;margin:0}#mobile-share-button a{display:block;height:100%;line-height:18px;width:100%}.mobile-share-panel-outer{background:#444}.mobile-share-panel-inner{background:#fff;border-bottom-left-radius:2px 2px;border-bottom-right-radius:2px 2px;border-radius:3px;-webkit-border-radius:3px;font-family:Arial;font-size:18px;color:#666}.mobile .mobile-share-panel-inner a{display:block;color:#666}.mobile-share-panel-title{background:#f5f5f5;border-bottom:1px solid #eee;border-top-left-radius:2px 2px;border-top-right-radius:2px 2px;height:25px;line-height:25px;padding:10px 10px 10px 20px}.mobile a.mobile-share-panel-button{background:#fff url(/img/mobile_share_icons4.png) no-repeat left !important;border-bottom:1px solid #eee;height:50px;line-height:30px;padding:10px 0 10px 65px;width:100%;-webkit-box-sizing:border-box}.mobile-share-panel-button-close{font-size:26px;float:right;height:25px;line-height:25px;text-align:center;width:25px}.mobile a.mobile-share-panel-button-email{background-position:10px 0 !important}.mobile a.mobile-share-panel-button-facebook{background-position:10px -50px !important}.mobile a.mobile-share-panel-button-twitter{background-position:10px -100px !important}.mobile a.mobile-share-panel-button-googleplus{background:#fff url(https://www.gstatic.com/images/icons/gplus-32.png) no-repeat left !important;background-position:19px 9px !important}.mobile a.mobile-share-panel-button-buzz{background-position:10px -150px !important;border-bottom-left-radius:2px 2px;border-bottom-right-radius:2px 2px}.svg-icon-24{height:24px;width:24px}form.gsc-search-box{font-size:13px;margin-top:0;margin-right:0;margin-bottom:4px;margin-left:0;width:100%}table.gsc-search-box{border-style:none;border-width:0;border-spacing:0 0;width:100%;margin-bottom:2px}table.gsc-search-box td{vertical-align:middle}table.gsc-search-box td.gsc-input{padding-right:12px}td.gsc-search-button{width:1%}td.gsc-clear-button{width:14px}input.gsc-search-button{margin-left:2px}input.gsc-input{padding:1px 6px;border:1px solid #ddd;width:99%} .quickedit {display:none;}

/* Content
----------------------------------------------- */
* {padding:0;margin:0;}html {scroll-behavior: smooth;}@media screen and (prefers-reduced-motion: reduce) {html {scroll-behavior: auto;}}body {font: $(body.font);color: $(body.text.color);background: $(body.background);padding: 0 $(content.shadow.spread) $(content.shadow.spread) $(content.shadow.spread);$(body.background.override)padding-bottom: 0px !important;}.full {padding: 0;}.full .content-outer {max-width: 100%;}.full .tabs-outer .tabs-inner .widget ul {max-width: 100%;margin: 0 auto;}.full .box-konten .row,.full .box-konten .head-feat {max-width: 1440px; margin: 0 auto;}.full .column-center-inner {padding: 0px !important;}.full .main {margin: 0 !important}#navbar { display: none; }html body $(page.width.selector) {max-width: 100%;width: $(page.width)}img {max-width: 100%}h1,h2,h3,h4,h5,h6 {margin-bottom: 20px}p {margin-top: 0}h1.txt-title {}h2.txt-title {}h3.txt-title {}p.txt-caption {font-size: 26px;letter-spacing: -1px;line-height: 1.4em;margin-bottom: 1.76471rem;}a:link {text-decoration: none;color: $(link.color)}a:visited {text-decoration: none;color: $(link.visited.color)}a:hover {text-decoration: underline;color: $(link.hover.color)}.content-outer {margin-bottom: 1px}.content-inner {padding: $(content.padding) $(content.padding.horizontal)}$(content.background.color.selector) {background-color: $(content.background.color)}.header-outer, .header-menu {background: $(header.background.color) $(header.background.gradient) repeat-x scroll 0 -400px;_background-image: none;text-align: center;}.Header h1 {font: $(header.font);color: $(header.text.color);text-shadow: $(header.shadow.offset.left) $(header.shadow.offset.top) $(header.shadow.spread) rgba(0, 0, 0, .2);line-height: 1.15em;letter-spacing: -.0625em}.Header h1 a {color: $(header.text.color)}.Header .description {font-size: $(description.text.size);color: $(description.text.color)}#header-inner img {max-width: 100%;height: auto;margin: 0 auto}.header-inner .Header .titlewrapper {padding: 22px $(header.padding) 0}.header-inner .Header .descriptionwrapper {padding: 0 $(header.padding)}.tabs-inner {padding: 0;background: $(tabs.background.color);}.tabs-inner .widget ul {_background-image: none;margin-top: $(tabs.margin.top)}.tabs-inner .widget li a {display: inline-block;padding: 15px 15px;font: $(tabs.font);color: $(tabs.text.color) }.tabs-inner .widget li.selected a, .tabs-inner .widget li a:hover {color: $(tabs.selected.text.color);background-color: $(tabs.selected.background.color);text-decoration: none }.section {margin: 0 }.cover .widget, .box-konten .widget {margin: 0 }.row {clear: both;padding: 0;margin: 0 }.col {display: block;float: left;margin: 0 0 0 1.6%;}.col:first-child {margin-left: 0 }.group:before, .group:after {content: "";display: table }.group:after {clear: both }.group {zoom: 1 }.kolom11 {width: 66.13% }.cover-kolom22 {width: 40% }.cover-kolom12 {width: 58.33% }.kolom22 {width: 100% }.kolom12 {width: 49.2% }.kolom-besar {width: 60.13% }.kolom-kecil {width: 38.26% }.kolom33 {width: 100% }.kolom23 {width: 66.13% }.kolom13 {width: 32.26% }.kolom44 {width: 100% }.kolom34 {width: 74.6% }.kolom24 {width: 49.2% }.kolom14 {width: 23.8% }.kolom66 {width: 100% }.kolom56 {width: 76.6666% }.kolom46 {width: 61.3333% }.kolom36 {width: 45.9999% }.kolom26 {width: 30.6666% }.kolom16 {width: 15.3333% }.kolomfull {width: 100% }@media only screen and (max-width:480px){.col{margin:1% 0}.kolom12,.kolom13,.kolom14,.kolom22,.kolom23,.kolom24,.kolom33,.kolom34,.kolom44{width:100%}.kolom16,.kolom26,.kolom36,.kolom46,.kolom56,.kolom66{width:50%}.cover-kolom12,.cover-kolom22,.kolom-besar,.kolom-kecil{width:100%}}.no-items {padding: 0!important;margin: 0!important }.cover {color: $(cover.text.color);background: $(cover.background.color) }.cover .w-cover {overflow: hidden }.cover .row {max-width: 100%;width: $(page.width);margin: auto }.cover img {display: inherit;margin: auto;}.cover h1, .cover h2 {font: $(cover.font);margin-bottom: .5em;padding: 0;line-height: 1.15em;letter-spacing: -.0625em }.cover p {font-size: 18px;margin: 0 0 30px;font-weight: normal }.cover1 {padding: 40px }.cover2 {padding: 40px }.cover3 {text-align: center;padding: 100px 40px;position: relative;clear: both }.cover3:before {content: ' ';display: block;position: absolute;left: 0;top: 0;width: 100%;height: 100%;z-index: 1;background: url(https://placeimg.com/960/480/any);background-size: cover;opacity: .5 }.cover3 .isi-cover3 {position: relative;z-index: 2 }.cover4 {padding: 70px 40px }.wrap-video {position: relative;padding-bottom: 56.25%;padding-top: 0;height: 0 }.wrap-video iframe {position: absolute;top: 0;left: 0;width: 100%;height: 100% }#featured-video4.is-sticky {position: fixed;top: 15px;left: auto;right: 15px;max-width: 280px;max-height: 158px;width: 280px;height: 158px;z-index: 9999;}.cover5 {padding: 40px;text-align: center }.cover5 .col {text-align: left }.cover5 .no-left {margin-left: 0 }.cover5 ul {list-style: none;padding: 0 }.cover5 li {padding-left: 1.3em !important;font-size: 24px;margin-bottom: 14px !important;}.cover5 li:before {content: "\f14a";font-family: FontAwesome;display: inline-block;margin-left: -1.3em;width: 1.3em }.cover6 {padding: 40px }.cover6 form {text-align: center;color: #fff;}.cover6 form fieldset {background: #333;border-radius: 5px;border: none;padding: 30px 30px 10px }.cover6 form fieldset .form-group {margin-bottom: 15px }.cover6 form fieldset .form-group .form-control {padding: 10px;border-radius: 5px;border: none;font-size: 16px;width: 100%;box-sizing: border-box }.cover6 form fieldset .form-group .btn {width: 100%;box-sizing: border-box;border: none }.cover6 span {font-size: 13px }.cover7 {text-align: center;padding: 100px 40px;position: relative;clear: both }.cover7:before {content: ' ';display: block;position: absolute;left: 0;top: 0;width: 100%;height: 100%;z-index: 1;background: url(https://placeimg.com/960/480/any);background-size: cover;opacity: .5 }.cover7 .isi-cover3 {position: relative;z-index: 2 }.cover8, .cover9 {padding: 40px;}.cover8 .wrap-video {margin-bottom: 30px;}.cover9 {position: relative;color: #fff;text-shadow: 0px 2px 1px rgba(0, 0, 0, 0.7) }.cover9:before {content: ' ';display: block;position: absolute;left: 0;top: 0;width: 100%;height: 100%;z-index: 1;background: url(https://2.bp.blogspot.com/-QwfGNabsfMw/WOjqF6XtqJI/AAAAAAAAAc0/rUF7aDReg1YUauzH1UZokxSplbiEPOvEwCLcB/s1600/bg-city.jpg) no-repeat;background-size: cover;}.cover9 .row {position: relative;z-index: 5;}.cover9 .isi {padding-left: 40px;padding-top: 50px;}.cover10,.cover11 {padding: 40px;}.cover10 {position: relative;color: #fff;text-shadow: 0px 2px 1px rgba(0, 0, 0, 0.7) }.cover10 .row {position: relative;z-index: 5;}.cover10 .isi {padding-top: 50px;}.cover10:before {content: ' ';display: block;position: absolute;left: 0;top: 0;width: 100%;height: 100%;z-index: 1;background: url(https://2.bp.blogspot.com/-nCqGaCVwelE/WQ3YrUgodmI/AAAAAAAAAjQ/pvI6ug0hN8wafRoVnFppaSU-BMmIZHWPgCLcB/s1600/bg-cover3.jpeg) no-repeat;background-size: cover;}.cover10 #clock-c9 {font-size: 30px;margin-bottom: 20px;}.cover10 .waktu {display: inline-block;font-size: 16px;margin: 10px;color: #fff;}.cover10 .waktu span {font-size: 6em;background: #fff;color: #111;border-radius: 5px;padding: 0 10px;text-shadow: 0px 10px 20px rgba(0, 0, 0, 0.36);}.cover10 hr {width: 10%;margin: 20px auto 20px;border: none;border-top: solid 1px #ffde00;}.cover11 {padding-top: 10em;padding-bottom: 10em;position: relative;}.cover11:before {content: ' ';display: block;position: absolute;left: 0;top: 0;width: 100%;height: 100%;z-index: 1;background: url(https://3.bp.blogspot.com/-jz_NF97FvQY/WRNlm5Gb1iI/AAAAAAAAAjk/Rqq7rN6FPsoKkmPblwQ7VmZ646hYHCxEACLcB/s1600/pexels-photo-325521.jpeg) bottom center no-repeat;background-size: cover;}.cover11 .full-row {position: relative;z-index: 6;}.cover11 h2 {}.cover12 {position: relative;height:95vh;min-height: 200px;overflow: hidden;}.cover12 .video-background {background: #000;top: 0;right: 0;bottom: 0;left: 0;z-index: -99;display: table;}.cover12 .video-foreground {opacity: 0.2;}.cover12 .video-foreground, .video-background iframe {position: absolute;top: 0;left: 0;width: 100%;height: 100%;pointer-events: none;}.cover12 .full-row {position: absolute;top: 50%;left: 50%;transform: translate(-50%,-50%);}@media (min-aspect-ratio: 16/9) {.cover12 .video-foreground {height: 300%;top: -100%;}}@media (max-aspect-ratio: 16/9) {.cover12 .video-foreground {width: 300%;left: -100%;}}.aroodam-content-1 {background: $(pemisah1.background.color);color: $(pemisah1.text.color) }.aroodam-content-2 {background: $(features.background.color);color: $(features.text.color) }.aroodam-content-3 {background: $(pemisah2.background.color);color: $(pemisah2.text.color) }.aroodam-content-4 {background: $(testimoni.background.color);color: $(testimoni.text.color) }.aroodam-content-5 {background: $(pemisah3.background.color);color: $(pemisah3.text.color) }.aroodam-content-6 {background: $(cta.background.color);color: $(cta.text.color) }.aroodam-content-7 {background: $(pemisah4.background.color);color: $(pemisah4.text.color) }.aroodam-content-8 {background: $(footer.background.color);color: $(footer.text.color) } .footer-global {background: $(footerglobal.background.color);color: $(footerglobal.text.color) } .footer-global h2.title {color: $(footerglobaltitle.text.color) !important; border-bottom: none !important;} .txt-center {text-align: center }.txt-left {text-align: left }.txt-miring {font-style: italic }.aroodam-content {color: #444444;background-color: #ffffff }.box-konten {padding: 0 }.pad40 {padding: 40px }.box-konten h1 {font-size: 55px;}.box-konten h2 {font-size: 48px;}.box-konten h2, .box-pricing h2 {margin-bottom: 15px;font-size: 48px;padding: 0;line-height: 1em;letter-spacing: -.0625em }.box-konten h2 span {font-family: playfair display;font-style: italic;font-weight: bold;}.box-konten h3 {margin-top: 10px;margin-bottom: 10px }.box-konten p {margin-top: 10px;margin-bottom: 1.76471rem;}.row .fa {font-size: 50px }.row .fa-kecil {font-size: 40px;float: left;margin-right: 20px }.feat-1 {padding: 40px 40px 20px }.feat-2 {padding: 40px 40px 20px }.feat-2 .list-box {padding: 0 20px;overflow: hidden;margin-bottom: 10px }.feat-2 .list-box .list-icon {width: 50px;height: 50px;float: left;margin: 10px }.feat-2 .list-box .list-isi {overflow: hidden;margin-right: 15px }.feat-3 {padding: 40px 40px 20px }.feat-3 img {border-radius: 3px }.feat-4 {padding: 40px 40px 20px }.feat-5 {padding: 40px 40px 20px }.feat-5 .feat-list {margin: 15px auto;overflow: hidden }.feat-6 {padding: 40px 40px 20px }.feat-7 {padding: 40px 40px 20px }.feat-7 .list-box {padding: 0 20px 0 0;overflow: hidden;margin-bottom: 10px }.feat-7 .list-box .list-icon {width: 50px;height: 50px;float: left;margin: 10px }.feat-7 .list-box .list-isi {overflow: hidden;margin-right: 15px }.feat-8 {padding: 40px 40px 20px }.feat-8 .fa {font-size: 30px;vertical-align: middle;margin-right: 10px }.feat-9 {padding: 40px 40px 20px }.feat-10 {padding: 0 }.feat-10 h3 {margin-bottom: .8em;font-size: 30px;padding: 0;line-height: 1.15em;letter-spacing: -.0625em }.feat-10 .feat-list {width: 100%;clear: both;display: inline-block;padding: 0px;}.feat-10 .feat-list .padding {padding: 30px;overflow: hidden;}.feat-10 .tukar {background: #fbefef;display: inline-block }.feat-10 .tukar .kolom13 {float: right;margin-left: 1.6% }.feat-10 .tukar .kolom23 {margin-left: 0 }.feat-10 .feat-list img {text-align: center }.feat-11 {padding: 40px 40px 20px;}.feat-11 .wrap-video {margin-bottom: 30px !important;padding-bottom: 28%;}.feat-11 .wrap-video iframe, .feat-13 .wrap-video iframe {height: 100%;padding-bottom: 10px;}.feat-12 {padding: 40px 40px 1px }.feat-13 {padding: 40px 40px 20px }.feat-13 .wrap-video {margin-bottom: 20px !important;padding-bottom: 28%;}.feat-13 .list-box {overflow: hidden;margin-bottom: 5px }.feat-13 .list-box .list-icon {width: 50px;height: 50px;float: left }.feat-13 .list-box .list-isi {overflow: hidden;margin-right: 15px }.feat-14 {padding: 40px 40px 20px }.feat-15 {padding: 40px }.feat-15 img {border-radius: 3px }.feat-16 {padding: 40px }.feat-17 {padding: 40px 40px 20px }.feat-17 ul {list-style: none;padding-left: 15px;margin: 0 }.feat-17 li:before {font-family: 'FontAwesome';content: '\f00c';margin: 0 10px 0 -26px;color: #f00 }.feat-17 li {margin-bottom: 15px;padding-left: 10px }.feat-18 {padding: 40px 40px 20px;background: #d35400;color: #fff;font-weight: bolder;text-shadow: 0 1px 1px #333 }.feat-18 .counter {font-size: 45px }.feat-19 {padding: 40px 40px 20px;background: #27ae60;color: #fff;font-weight: bolder;text-shadow: 0 1px 1px #333 }.feat-19 .counter {font-size: 45px }.feat-20 {padding: 40px 40px 20px;background: #fddfc6 }.feat-20 span {font-size: 35px }.feat-20 .btn {margin-left: 20px }.feat-21 {padding: 40px;background: #8e44ad;color: #fff }.feat-21 h2 {margin-bottom: 0 }.feat-22 {padding: 40px }.feat-22 a:hover {opacity: .8 }.feat-23 {padding: 40px;background: #fff;}.feat-23 .fb-comments {background: #fff;}.feat-24 {padding: 40px;background: #0797eb;}.feat-24:hover {background: #17aaff;}.feat-24 h2 {margin-bottom: 0px;}.feat-24 h2 a {font-weight: 100;color: #fff;}.feat-24 h2 a:hover {text-decoration: none;}.feat-24 h2 span {margin:0 30px;font-weight: 100;}.modalDialog {position: fixed;font-family: Arial, Helvetica, sans-serif;top: 0;right: 0;bottom: 0;left: 0;background: rgba(0, 0, 0, 0.8);z-index: 99999;opacity:0;-webkit-transition: opacity 400ms ease-in;-moz-transition: opacity 400ms ease-in;transition: opacity 400ms ease-in;pointer-events: none;}.modalDialog:target {opacity:1;pointer-events: auto;}.modalDialog > div {max-width: 500px;height: 315px;position: relative;margin: 15% auto;padding: 0;background: #fff;background: -moz-linear-gradient(#fff, #999);background: -webkit-linear-gradient(#fff, #999);background: -o-linear-gradient(#fff, #999);}.close {background: #fff;color: #000 !important;line-height: 25px;position: absolute;right: -12px;text-align: center;top: -10px;width: 24px;text-decoration: none;font-weight: bold;-webkit-border-radius: 12px;-moz-border-radius: 12px;border-radius: 12px;-moz-box-shadow: 1px 1px 3px #000;-webkit-box-shadow: 1px 1px 3px #000;box-shadow: 1px 1px 3px #000;}.close:hover {background: #00d9ff;}.feat-25 {}.sss {height: 0;margin: 0;padding: 0;position: relative;display: block;overflow: hidden;}.ssslide {width: 100%;margin: 0;padding: 0;position: absolute;top: 0;left: 0;display: none;overflow: hidden;}.ssslide img {max-width: 100%;height: auto;margin: 0;padding: 0;position: relative;display: block;}.sssnext, .sssprev {width: 25px;height: 100%;margin: 0;position: absolute;top: 0;background: url('https://1.bp.blogspot.com/-10VvZ7Holis/WN5_el8inOI/AAAAAAAAAZ4/jBC7F4ZfkT8MInInfgABwL17PDPRu2JywCLcB/s1600/arr.png') no-repeat;}.sssprev {left: 3%;background-position: 0 50%;}.sssnext {right: 3%;background-position: -26px 50%;}.sssprev:hover, .sssnext:hover {cursor: pointer;}.feat-26,.feat-27,.feat-28 {padding: 40px;background: #fff;}.feat-26 .konten-tabs {display: -webkit-flex;display: -ms-flexbox;display: flex;margin-bottom: 30px;}.feat-26 .konten-tabs li {color: #444;margin: 0px;flex: 1;width: 25%;transition: background 0.2s;position: relative;}.feat-26 .konten-tabs li .fa {margin-bottom: 15px;}.feat-26 .konten-tabs .current:after, .feat-26 .konten-tabs .current:before {top: 100%;left: 50%;border: solid transparent;content: " ";height: 0;width: 0;position: absolute;pointer-events: none;border-color: rgba(52, 152, 219, 0);border-top-color: #3498db;border-width: 15px;margin-left: -15px;}.feat-27 .kolom23 {margin-left:0;}.feat-28 h3 {margin-bottom: .8em;font-size: 30px;padding: 0;line-height: 1.15em;letter-spacing: -.0625em;}.feat-29 {padding: 40px;}.feat-30 {}.feat-30 .row{display: -webkit-flex;display: -ms-flexbox;display: flex;overflow: hidden;}.feat-30 .row .col {color: #111;margin: 0px;flex: 1;background: #177af4;width: 25%;-webkit-box-shadow: inset 1px 0px 0px 0px rgba(0,0,0,0.1);-moz-box-shadow: inset 1px 0px 0px 0px rgba(0,0,0,0.1);box-shadow: inset 1px 0px 0px 0px rgba(0,0,0,0.1);-webkit-transition: background 0.2s;transition: background 0.2s;}.feat-30 .row .col:first-child {box-shadow: none;background: #F8F087;}.feat-30 .row .col:nth-child(2) {background: #B7E3C0;}.feat-30 .row .col:nth-child(3) {background: #B8D0DD;}.feat-30 .row .col:nth-child(4) {background: #DBBAE5;}.feat-30 .row .col:nth-child(5) {background: #F39DD4;}.feat-30 .row .col:hover {background: #4294f9;color: #fff;}.feat-30 .wrap {padding: 20px;}.feat-30 hr {border: none;border-top: 1px solid #fff;margin: 25px 30%;}.feat-31 {padding: 40px;}.feat-31 h4 {margin-top: 10px;}.feat-31 .col .wrap-img {display: inline-block;overflow: hidden;}.feat-31 .col .wrap-img img {width: 100%;}.feat-32 {}.feat-32 .head-feat {padding: 40px 20px 40px 70px;}.feat-32 .feat-list {overflow:hidden;position: relative;}.feat-32 .feat-list .col {padding-bottom: 100%;margin-bottom: -100%;}.feat-32 h3 {font-size: 30px;}.feat-32 .feat-list .col.gkanan {text-align: right;line-height: 0;position: static;}.feat-32 .feat-list .col.gkanan img {}.feat-33 {}.feat-33 .head-feat {padding: 40px 70px 40px 20px;}.feat-33 .feat-list {overflow:hidden;position: relative;}.feat-33 .feat-list .col {padding-bottom: 100%;margin-bottom: -100%;}.feat-33 .feat-list .kolom23 {float: right;}.feat-33 h3 {font-size: 30px;}.feat-33 .feat-list .col.gkiri {text-align: left;line-height: 0;margin-left: 0;}.feat-33 .feat-list .col.gkiri img {}.feat-34 {padding: 40px 40px 0 40px;}.feat-34 h3 {font-size: 30px;}.feat-34 .feat-list {overflow:hidden;position: relative;}.feat-32,.feat-33,.feat-34 {border-bottom: solid 1px #f1f1f1;}.feat-34 .feat-list .col.gbawah {line-height: 0;}.feat-34 .feat-list .col.gbawah img {position: relative;bottom:0;}.feat-35 {padding: 40px;}.feat-35 .col:first-child {text-align: right;margin-top: 50px;}.feat-35 .col:last-child {margin-top: 50px;}.feat-36 {padding: 40px;}.feat-36 .video-slider iframe {height: 500px;}.feat-37 {padding: 40px 40px 0px 40px;border-bottom: solid 1px #f1f1f1;}.feat-37 .head-feat {padding-bottom: 40px;padding-top: 30px;}.feat-37 .feat-list.tukar .teks{float: right;margin-left: 1.6%;}.feat-37 .feat-list.tukar .gbawah{margin-left: 0;}.feat-37 .feat-list {overflow:hidden;padding-top: 30px;border-bottom: solid 1px #f1f1f1;}.feat-37 .feat-list .gbawah {line-height: 0;}.feat-37 .head-feat {padding-bottom:0;}.feat-38,.feat-39,.feat-40 {padding: 40px;}.feat-39 .step {padding: 0 20px;position: relative;}.feat-39 .row .col:nth-child(2) .step {padding: 0 20px;}.feat-39 .row .col:nth-child(2) .step:before {content: "";width: 21px;height: 39px;background: url("https://2.bp.blogspot.com/-hBqikdXy3Kk/WPK2muNQwoI/AAAAAAAAAg0/K8TkndIAgB8WaHZEvLQnskAd_fPLLAjMwCLcB/s1600/step-icon.png") no-repeat ;left: 0px;top: 20%;position: absolute;display: inline-block;}.feat-39 .row .col:nth-child(2) .step:after {content: "";width: 21px;height: 39px;background: url("https://2.bp.blogspot.com/-hBqikdXy3Kk/WPK2muNQwoI/AAAAAAAAAg0/K8TkndIAgB8WaHZEvLQnskAd_fPLLAjMwCLcB/s1600/step-icon.png") no-repeat ;right: 0px;bottom: 53%;position: absolute;display: inline-block;}.feat-40 .row .step {padding: 20px;position: relative;}.feat-40 .row .step .no {background: #333;margin: 0 auto 20px;width: 40px;height: 40px;border-radius: 30px;font-size: 25px;line-height: 40px;color: #fff;}.feat-40 .row .col:nth-child(3n+1) {margin-left: 0px;}.feat-40 .row .col:nth-child(3) .step:after {content: "";width: 21px;height: 39px;left: 0px;bottom: 0;position: absolute;display: inline-block;}.feat-40 .row .col:nth-child(3n+2) .step:before {content: "";width: 21px;height: 39px;background: url("https://2.bp.blogspot.com/-hBqikdXy3Kk/WPK2muNQwoI/AAAAAAAAAg0/K8TkndIAgB8WaHZEvLQnskAd_fPLLAjMwCLcB/s1600/step-icon.png") no-repeat ;left: 0px;top: 32%;position: absolute;display: inline-block;}.feat-40 .row .col:nth-child(3n+2) .step:after {content: "";width: 21px;height: 39px;background: url("https://2.bp.blogspot.com/-hBqikdXy3Kk/WPK2muNQwoI/AAAAAAAAAg0/K8TkndIAgB8WaHZEvLQnskAd_fPLLAjMwCLcB/s1600/step-icon.png") no-repeat ;right: 0px;bottom: 53%;position: absolute;display: inline-block;}.feat-41 {}.feat-41 .head-feat {padding-top: 40px;}.feat-41 .row{display: -webkit-flex;display: -ms-flexbox;display: flex;overflow: hidden;}.feat-41 .row .col {color: #333;margin: 0px;flex: 1;display: inline-grid;background: #fede00;width: 25%;-webkit-box-shadow: inset 1px 0px 0px 0px rgba(0,0,0,0.1);-moz-box-shadow: inset 1px 0px 0px 0px rgba(0,0,0,0.1);box-shadow: inset 1px 0px 0px 0px rgba(0,0,0,0.1);-webkit-transition: background 0.2s;transition: background 0.2s;}.feat-41 .row .col:first-child {box-shadow: none;}.feat-41 .row .col:hover {background: #a9e200;}.feat-41 .wrap {padding: 20px;display: flex;flex-direction: column;justify-content: center;align-items: center;}.feat-41 h3 {font-size: 25px;}.feat-42 {}.feat-42 .head-feat {padding-top: 40px;}.feat-42 .row{display: -webkit-flex;display: -ms-flexbox;display: flex;overflow: hidden;}.feat-42 .row .col {color: #333;margin: 0px;flex: 1;display: inline-grid;background: #00cbf4;width: 50%;-webkit-box-shadow: inset 1px 0px 0px 0px rgba(0,0,0,0.1);-moz-box-shadow: inset 1px 0px 0px 0px rgba(0,0,0,0.1);box-shadow: inset 1px 0px 0px 0px rgba(0,0,0,0.1);-webkit-transition: background 0.2s;transition: background 0.2s;}.feat-42 .row .col:first-child {box-shadow: none;}.feat-42 .row.tukar .col:first-child {margin-left: auto;order: 2;}.feat-42 .row .col:hover {background: #ffcf2d;}.feat-42 .wrap {padding: 20px;display: flex;flex-direction: column;justify-content: center;align-items: center;}.feat-42 h3 {font-size: 25px;}.feat-43 {padding: 40px;}.timeline {position: relative;list-style: none;margin: 30px auto !important;padding: 0 !important;}.timeline:before {content: " ";position: absolute;left: 23%;top: -20px;height: 103%;border-right: 3px solid #ffcf26;margin-top: -10px;}.timeline li {list-style: none !important;margin: 0 0 3em;padding: 0 !important;overflow: hidden;}.timeline span.date {font-size: 1em;color: inherit;text-align: right;padding-right: 5%;padding-top: 10px;padding-bottom: 10px;float: left;width: 15%;background: #ffcf26;position: relative;-webkit-border-top-left-radius: 15px;-webkit-border-bottom-left-radius: 15px;-moz-border-radius-topleft: 15px;-moz-border-radius-bottomleft: 15px;border-top-left-radius: 15px;border-bottom-left-radius: 15px;}.timeline span.date:after {left: 100%;top: 50%;border: solid transparent;content: " ";height: 0;width: 0;position: absolute;pointer-events: none;border-color: rgba(255, 207, 38, 0);border-left-color: #ffcf26;border-width: 5px;margin-top: -5px;}.timeline .dot {position: absolute;left: 23%;color: #fff;background: #ffcf27;width: 10px;height: 10px;border-radius: 100%;margin-top: 10px;margin-left: -8px;border: solid 5px #fff;}.timeline .wrap-timeline {width: 74%;float: right;}.timeline h3 {font-size: 25px;margin-bottom: 15px;margin-top: 0px;}.full-list {list-style: none;padding: 0 !important;}.full-list li {padding: 15px 25px !important;border: solid 2px #ecf0f1;background: #ecf0f1;color: #333;}.full-list li:before {font-family: 'FontAwesome';content: '\f046';color: #333;margin:0 5px 0 -15px;}ul.konten-tabs, ul.v-tabs, ul.icon-tabs{margin: 0px;padding: 0px;list-style: none;text-align: center;}ul.icon-tabs {box-shadow: inset 0px -2px 0px #f1f1f1;margin-bottom: 2px;}ul.konten-tabs li, ul.v-tabs li, ul.icon-tabs li{background: none;color: #222;display: inline-block;padding: 10px 15px !important;cursor: pointer;margin-bottom: 0px !important;}ul.v-tabs li {display: block;text-align: left;}ul.icon-tabs li i {margin-bottom: 15px;}ul.konten-tabs li.current, ul.v-tabs li.current{background: #3498db;color: #fff;}ul.icon-tabs li.current {border-bottom: solid 2px #2196f3;}ul.icon-tabs li.current .fa {color: #2196f3}.tab-content, .v-content, .icon-content{display: none;background: #fff;padding: 20px 0px;}.v-content {padding: 0px 20px;}.tab-content.current, .v-content.current, .icon-content.current{display: inherit;}.v-content.current {border-top: none;border-left: solid 2px #3498db;}.merah {color: #e74c3c }.hijau {color: #2ecc71 }.orange {color: #f39c12 }.biru {color: #3498db }.ungu {color: #8e44ad }.kuning {color: #ffde00 }.pricing .price {background: #fff;list-style-type: none;border: 1px solid #eee;margin: 0;padding: 0;-webkit-transition: .3s;transition: .3s }.pricing .price:hover {box-shadow: 0 8px 12px 0 rgba(0, 0, 0, 0.2) }.pricing .price .header {color: white;font-size: 25px;border-bottom: none }.pricing .price .desc {color: #fff;padding-top: 0;border-bottom: none }.pricing .price li {border-bottom: 1px solid #eee;padding: 15px 20px;text-align: center;margin-bottom: 0 }.pricing .price li:before {list-style: none;content: '';margin: auto }.pricing .price .harga span {font-size: 60px;font-weight: bold;letter-spacing: -.0525em }.pricing .table-harga-1 .price .header {background: #27ae60 }.pricing .table-harga-2 .price .header {background: #e67e22 }.pricing .table-harga-3 .price .header {background: #8e44ad }.pricing .table-harga-1 .price .desc {background: #27ae60 }.pricing .table-harga-2 .price .desc {background: #e67e22 }.pricing .table-harga-3 .price .desc {background: #8e44ad }.pricing .table-harga-1 .price .harga {background: #e5fcee }.pricing .table-harga-2 .price .harga {background: #fbefe2 }.pricing .table-harga-3 .price .harga {background: #f5e4fd }.pricing .btn {margin-bottom: 0 }.pricing-1 {padding: 40px }.pricing-2 {padding: 40px }.pricing-2 .table-harga-1 {padding-left: 4em;padding-right: 4em }.pricing-2 .table-harga-1 .price .header {font-size: 48px;font-weight: bold;line-height: 1.15em;letter-spacing: -.0625em }.pricing-2 .table-harga-1 .price .harga strike {font-size: 30px;color: #1abc9c;font-weight: bold }.pricing-2 .table-harga-1 .price .harga {background: #fff }.pricing-2 .table-harga-1 .price .harga span {font-size: 5em;color: #e74c3c }.pricing-2 .btn {border-radius: 50px;font-size: 30px;padding: 20px 50px }.pricing-3 {padding: 40px }.pricing-3 .price li {text-align: left }.pricing-3 .table-harga-1 .price .header {background: #fff;color: #2ecc71;font-weight: bold }.pricing-3 .table-harga-1 .price .header span {border-bottom: solid 7px #2ecc71;padding-bottom: 12px }.pricing-3 .table-harga-2 .price .header {background: #fff;color: #f1c40f;font-weight: bold }.pricing-3 .table-harga-2 .price .header span {border-bottom: solid 7px #f1c40f;padding-bottom: 12px }.pricing-3 .table-harga-3 .price .header {background: #fff;color: #e74c3c;font-weight: bold }.pricing-3 .table-harga-3 .price .header span {border-bottom: solid 7px #e74c3c;padding-bottom: 12px }.pricing-3 .table-harga-1 .price .desc {background: #fff;color: #666;padding-top: 20px;padding-bottom: 0 }.pricing-3 .table-harga-2 .price .desc {background: #fff;color: #666;padding-top: 20px;padding-bottom: 0 }.pricing-3 .table-harga-3 .price .desc {background: #fff;color: #666;padding-top: 20px;padding-bottom: 0 }.pricing-3 .table-harga-1 .price .harga {background: #fff;color: #2ecc71;border-bottom: none }.pricing-3 .table-harga-2 .price .harga {background: #fff;color: #f1c40f;border-bottom: none }.pricing-3 .table-harga-3 .price .harga {background: #fff;color: #e74c3c;border-bottom: none }.pricing-3 .price li.b-list {padding: 5px 20px;border-bottom: none }.pricing-4,.pricing-5 {padding: 40px;}.tampilkan {margin-bottom: -1px;}.tampilkan ul.plan-tabs {display: none;width: 100%;border-collapse: collapse;border-top: 1px solid #e5e5e5;border-bottom: none;}.tampilkan ul.plan-tabs button.t1.aktif {background: #e5fcee;}.tampilkan ul.plan-tabs button.t2.aktif {background: #fbefe2;}.tampilkan ul.plan-tabs button.t3.aktif {background: #f5e4fd;}.tampilkan ul.plan-tabs li{display: table-cell;border-left: 1px solid #e5e5e5;border-right: 1px solid #e5e5e5;padding: 0;}.tampilkan ul.plan-tabs li button{width: 100%;border:none;padding: 10px;background: #fff;}.tampilkan ul.plan-tabs li button.aktif{width: 100%;border:none;background: #eee;}.tabel-harga {width: 100%;border-collapse: collapse;-webkit-text-size-adjust: 100%;}.tabel-harga thead .heading {font-size: 18px;font-weight: bold;margin-bottom: 10px;}.tabel-harga tbody {background: #fff;}.tabel-harga th, .tabel-harga td {padding: 10px 15px;border: 1px solid #e5e5e5;font-weight: normal;}.tabel-harga thead th {width: 22.22222%;}.tabel-harga thead p {font-size: 13px;}.tabel-harga thead .p0,.tabel-harga thead .pa0 {border-top: none;border-left: none;}.tabel-harga thead .p1,.tabel-harga thead .pa1 {background: #e5fcee;}.tabel-harga thead .p2,.tabel-harga thead .pa2 {background: #fbefe2;}.tabel-harga thead .p3 {background: #f5e4fd;}.tabel-harga thead th:first-child {width: 33.33333%;}.tabel-harga tbody {color: #999;}.tabel-harga tbody th {text-align:left;}.tabel-harga tbody .harga {color: #333;text-align: center;font-size: 35px;font-weight: bold;}.tabel-harga tbody .h1,.tabel-harga tbody .ha1 {background: #27ae60;color: #fff;}.tabel-harga tbody .h2,.tabel-harga tbody .ha2 {background: #e67e22;color: #fff;}.tabel-harga tbody .h3 {background: #8e44ad;color: #fff;}.tabel-harga tbody.list td {background: #fff;color: #333;}.tabel-harga tbody .fitur {font-weight: bold;color: #333;}.tabel-harga tbody td {text-align:center;}.tabel-harga tbody .fa {font-size: 20px;}.cta-1 {padding: 40px }.cta-1 h2 {font-size: 30px }.cta-1 h3 {font-size: 40px }.cta-1 .kotak-promo {margin: 30px auto;overflow: hidden;width: 500px;clear: both }.cta-1 .kotak-promo .harga-asli {width: 100px;float: left;font-size: 40px;position: relative;color: #888 }.cta-1 .kotak-promo .harga-asli .harga-coret {position: absolute;width: 100px;top: 5px }.cta-1 .kotak-promo .harga-baru {width: 390px;float: left;font-size: 60px;font-weight: bolder;color: #e93a5b;line-height: 50px;text-align: center }.cta-1 .order {clear: both }.cta-1 .btn {font-size: 30px;border-radius: 50px;padding-left: 40px;padding-right: 40px }@keyframes blink {0% {color: red }100% {color: orange }}@-webkit-keyframes blink {0% {color: red }100% {color: orange }}.blink {-webkit-animation: blink 1s linear infinite;-moz-animation: blink 1s linear infinite;animation: blink 1s linear infinite }.cta-2 {padding: 40px }.cta-2 .order {margin-top: 20px;margin-bottom: 20px }.cta-2 .btn {font-size: 40px }.cta-3 {padding: 40px;background: #faf6bd }.cta-3 .box-harga {max-width: 400px;margin: 20px auto;background: #fff;outline: 6px dashed #ffd200;box-shadow: 0 0 0 6px #EA3556;animation: 1s animateBorderOne ease infinite }.cta-3 .box-harga .harga {font-size: 60px;font-weight: bold;padding-top: 20px;padding-bottom: 20px;border-bottom: dashed 3px #eb1e2a;color: #e74c3c }.cta-3 .box-harga .order {padding: 20px }.cta-3 .btn {font-size: 30px }.cta-3 .box-harga .pembayaran {padding: 0 20px 20px }@keyframes animateBorderOne {to {outline: 6px dashed #EA3556;box-shadow: 0 0 0 6px #ffd200 }}.cta-4 {padding: 40px;position: relative;color: #fff;overflow: hidden;background: #7f8c8d }.cta-4 h2 {font-size: 30px;text-shadow: 1px 1px 1px #333 }.cta-4:before {content: ' ';display: block;position: absolute;left: 0;top: 0;width: 100%;height: 100%;z-index: 1;opacity: .5;background: url(https://placeimg.com/960/480/arch);background-size: cover;}.cta-4 .txt-caption {color: #fff;text-shadow: 1px 1px 1px #333 }.cta-4 .isi {position: relative;z-index: 2 }.cta-5 {padding: 40px;color: #fff;position: relative }.cta-5:before {content: ' ';display: block;position: absolute;left: 0;top: 0;width: 100%;height: 100%;z-index: 1;background: url(https://placeimg.com/960/480/any);background-size: cover;opacity: .5 }.cta-5 .isi {position: relative;z-index: 2 }.cta-5 .txt-caption {color: #fff }.cta-5 .form-subscribe fieldset {display: inline-block;border: none;padding: 10px;background: rgba(0, 0, 0, .3);border-radius: 5px;box-sizing: border-box }.cta-5 .form-subscribe fieldset .form-group {float: left }.cta-5 .form-subscribe fieldset .form-group .input-md {font-size: 16px;margin: 0 7px;padding: 15px 20px;border-radius: 5px;border: none }.cta-5 .form-subscribe button {border: none;margin: 0 7px }.cta-5 .btn {font-weight: bold }.cta-6 {padding: 40px;color: #fff;background: #2860b3;position: relative }.cta-6:before {content: ' ';display: block;position: absolute;left: 0;top: 0;width: 100%;height: 100%;z-index: 1;background: url(https://placeimg.com/960/480/any);background-size: cover;opacity: .5 }.cta-6 .isi {position: relative;z-index: 2 }.cta-6 .txt-caption {color: #fff }.cta-6 .form-subscribe fieldset {display: inline-block;border: none;padding: 10px;background: rgba(0, 0, 0, .3);border-radius: 5px;box-sizing: border-box }.cta-6 .form-subscribe fieldset .form-group {float: left }.cta-6 .form-subscribe fieldset .form-group .input-md {font-size: 16px;margin: 0 7px;padding: 15px 20px;border-radius: 5px;border: none }.cta-6 .form-subscribe button {border: none;margin: 0 7px }.cta-6 .btn {font-weight: bold }.cta-7 {color: #333 }.cta-7:before {background: none }.cta-7 h2 {font-size: 30px }.cta-7 .txt-caption {color: #333;font-size: 20px }.cta-7 fieldset {background: none!important }.cta-7 .form-subscribe fieldset .form-group .input-md {background: #eee;width: 300px }.cta-7 button {}.cta-8 {color: #333 }.cta-8 h2 {font-size: 30px }.cta-8:before {background: none }.cta-8 .txt-caption {color: #333;font-size: 20px }.cta-8 fieldset {background: none!important }.cta-8 .form-subscribe fieldset .form-group .input-md {background: #eee }.cta-8 button {background: #0c71c6 }.cta-9 {padding: 40px;}.cta-9 .order a {margin: 5px;width: 75px;padding: 10px;color: #fff;}.cta-9 .btn-call {background:#2dc100;}.cta-9 .btn-sms {background:#4673e6;}.cta-9 .btn-wa {background:#65bc54;}.cta-9 .btn-bbm {background:#282828;}.cta-9 .btn-ln {background:#3acd01;}.cta-9 .btn-tele {background:#64a9dc;}.cta-9 .btn-wechat {background:#00c80f;}.cta-10 a.btn {color: #fff;}.cta-11 {padding: 40px;}.cta-12 {padding: 40px;}.cta-12 {background: #B24592;background: -webkit-linear-gradient(to top, #F15F79, #B24592);background: linear-gradient(to top, #F15F79, #B24592);color: #fff;}.cta-12 h1 {font-size: 60px;}.cta-12 h2 {font-weight: normal;}.cta-12 #clock {font-size: 30px;margin-bottom: 20px;}.cta-12 .waktu {display: inline-block;font-size: 16px;margin: 10px;}.cta-12 .waktu span {font-size: 6em;text-shadow: 0px 10px 20px rgba(0, 0, 0, 0.36);}.cta-12 .btn {box-shadow: 0px 10px 20px rgba(0, 0, 0, 0.36);}.cta-12 .btn-kuning {background: #ffde00;color: #333 !important;}.cta-13 {}.cta-13 .fbm {position: fixed;bottom: 20px;right: 20px;z-index: 1000;}.cta-13 .fbm img {-webkit-filter: drop-shadow(0px 0px 5px #2982fc);filter: drop-shadow(0px 0px 5px #2982fc);cursor: pointer;}.cta-13 .bubble {position: absolute;display:none;bottom: 80px;right: 0px;width: 250px;height: 300px;padding: 0px;background: #fff;-webkit-filter: drop-shadow(0px 0px 5px #2982fc);filter: drop-shadow(0px 0px 5px #2982fc);}.bubble:after {content: '';position: absolute;border-style: solid;border-width: 13px 12px 0;border-color: #FFFFFF transparent;display: block;width: 0;z-index: 1;bottom: -13px;left: 213px;}#slidebox{width:400px;height:auto;background-color:#fff;border-top:5px solid blue;position:fixed;bottom:0px;right:-430px;-moz-box-shadow:-2px 0px 5px #aaa;-webkit-box-shadow:-2px 0px 5px #aaa;box-shadow:-2px 0px 5px #aaa;z-index: 1000;}.wrap-slidebox {padding: 5px;text-align:center }#slidebox .close{width:13px;height:13px;position:absolute;cursor:pointer;top:10px;right:10px;}#slidebox a.close:hover{background-position:0px -13px;}.cta-10 .btn {width: 37px;font-size:8px;padding: 5px;margin: 2px 0px;}.cta-10 .btn img {width: 16px;}.cta-10 .btn-call {background:#2dc100;}.cta-10 .btn-sms {background:#4673e6;}.cta-10 .btn-wa {background:#65bc54;}.cta-10 .btn-bbm {background:#282828;}.cta-10 .btn-ln {background:#3acd01;}.cta-10 .btn-tele {background:#64a9dc;}.cta-10 .btn-wechat {background:#00c80f;}.cta-14,.cta-15,.cta-16 {padding: 40px;}.cta-14 #clock2, .cta-15 #clock3 {font-size: 20px;margin-bottom: 20px;}.cta-14 .waktu,.cta-15 .waktu {display: inline-block;font-size: 16px;margin: 10px;}.cta-14 .waktu span,.cta-15 .waktu span {font-size: 4em;}.cta-15 .waktu {position: relative;background: #333;color: #fff;padding: 10px;border-radius: 5px;}.cta-15 .waktu:before {content: '';border-top: solid 2px #fff;top: 50px;}.cta-16 img {vertical-align: middle;}.cta-16 .order .btn {color: #fff;}.cta-16 .order .btn-call {background: #00c600;}.cta-16 .order .btn-sms {background: #923fbf;}.cta-16 .order .btn-wa {background: #009c3a;}.cta-16 .order .btn-bbm {background: #000000;}.cta-16 .order .btn-ln {background: #00d200;}.cta-16 .order .btn-tele {background: #0089d3;}.cta-16 .order .btn-wechat {background: #00c600;}.cta-17 {position: fixed;width: 100%;display: block;bottom: 0;left: 0;z-index: 999;}.cta-17 .w-social {display: flex;justify-content: space-between;}.cta-17 .btn {background: rgba(0, 0, 0, 0.7);display: inline-block;text-align: center;flex-basis: 20%;padding: 10px;margin: 0px;border-radius: 0;font-size: 13px;color: #fff;}.cta-17 .btn:hover {background: rgba(255, 255, 255, 0.7);color: #000;}.cta-17 .btn img {vertical-align: middle;width: 20px;}.testimoni-1 {padding: 40px }.testimoni-1 .ava {width: 32px;height: 32px;overflow: hidden;margin: auto;border-radius: 50px }.testimoni-2 {padding: 40px 40px 20px;}.testimoni-2 h2 {font-size: 30px }.testimoni-2 .txt-caption {font-size: 20px }.testimoni-2 .ava {width: 32px;height: 32px;overflow: hidden;margin: auto;border-radius: 50px }.testimoni-3 .ava {width: 50px;height: 50px }.testimoni-3 p {font-size: 14px;font-weight: 400;font-style: normal;font-size: 13px;line-height: 145%;}.testimoni-4 {padding: 40px;background: #f9f9f9;}.testimoni-4 .ava {width: 250px;height: 250px;overflow: hidden;margin: auto;border-radius: 250px }.testimoni-4 .isi-testi {background: #fff;padding: 20px;color: #333;border-radius: 10px;position: relative;margin-bottom: 30px;margin-top: 30px }.testimoni-4 .isi-testi:after {top: 100%;left: 10%;border: solid transparent;content: " ";height: 0;width: 0;position: absolute;pointer-events: none;border-color: rgba(255, 255, 255, 0);border-top-color: #ffffff;border-width: 20px;margin-left: -20px }.testimoni-4 .tukar .kolom-kecil {float: right }.testimoni-4 .tukar .isi-testi:after {top: 100%;left: 90% }.testimoni-4 .tukar {text-align: right }.testimoni-5 {padding: 40px;}.testimoni-5 .ava {width: 100px;height: 100px;overflow: hidden;margin: 20px auto;border-radius: 250px }.testimoni-5 .txt-miring {margin-top: 20px;margin-bottom: 20px;}.testimoni-6 {padding: 40px;}.testimoni-6 .isi-testi {padding: 0 80px;}.testimoni-6 .ssslide img {margin: 0 auto !important;}.testimoni-7 {padding: 40px;background: #f9f9f9;}.testimoni-7 .ssslide {position: relative;}.testimoni-7 .ava {width: 250px;height: 250px;overflow: hidden;margin: auto;border-radius: 250px }.testimoni-7 .isi-testi {background: #fff;padding: 20px;color: #333;border-radius: 10px;position: relative;margin-bottom: 30px;margin-top: 30px }.testimoni-7 .isi-testi:after {top: 100%;left: 10%;border: solid transparent;content: " ";height: 0;width: 0;position: absolute;pointer-events: none;border-color: rgba(255, 255, 255, 0);border-top-color: #ffffff;border-width: 20px;margin-left: -20px }.testimoni-7 .tukar .kolom-kecil {float: right }.testimoni-7 .tukar .isi-testi:after {top: 100%;left: 90% }.testimoni-7 .tukar {text-align: right }.team-1 {padding: 40px }.team-1 .ava {width: 170px;height: 170px;overflow: hidden;margin: 20px auto;border-radius: 170px }.team-1 p {margin-bottom: 10px }.team-1 .fa {font-size: 20px;margin: 2px;color: #999 }.team-2 {padding: 40px }.team-2 .ava {width: 270px;height: 270px;overflow: hidden;margin: 20px auto;border-radius: 270px }.team-2 p {margin-bottom: 10px }.team-2 .fa {font-size: 20px;margin: 2px;color: #999 }.team-3 {padding: 40px }.team-3 .ava {width: 210px;height: 210px;overflow: hidden;margin: 20px auto;border-radius: 270px }.team-3 .fa {font-size: 20px;margin: 2px;color: #999 }.team-4 {padding: 40px }.team-4 .ava {width: 270px;height: 270px;overflow: hidden;margin: 20px auto;border-radius: 270px }.team-4 p {margin-bottom: 10px }.team-4 .fa {font-size: 20px;margin: 2px;color: #999 }.faq-1, .faq-2, .faq-3 {padding: 40px }.faq-1 .col {margin-bottom: 0 }button.accordion {position: relative; background-color: #f5f5f5;color: #444;cursor: pointer;padding: 18px;width: 100%;border: none;text-align: left;outline: none;font-size: 16px;font-weight: bold;transition: 0.4s;}button.accordion.active, button.accordion:hover {background-color: #f1f1f1;}button.accordion:after {position: absolute; right: 10px; top: 17px; content: '\002B';color: #777;font-weight: bold;float: right;margin-left: 15px;}button.accordion.active:after {content: "\2212";}div.panel {padding: 0 18px;background: rgba(255, 255, 255, 0.5);max-height: 0;overflow: hidden;transition: max-height 0.2s ease-out;}.footer-1 {padding: 40px }.footer-1 h2 {font-size: 30px }.footer-1 ul {list-style: none;padding: 0 }.footer-1 li {display: inline;margin: 10px }.footer-1 li:before {content: ''!important }.footer-1 a {color: #999 }.footer-2 {padding: 40px }.footer-2 .social {margin-top: 20px }.footer-2 .social img {margin: 7px }.footer-2 .social a {opacity: .8 }.footer-2 .social a:hover {opacity: 1 }.footer-3 {padding: 40px }.footer-3 h2 {font-size: 25px }.footer-3 .media img {margin: 10px;filter: grayscale(100%) }.footer-3 .media img:hover {filter: grayscale(0%) }.footer-4 {padding: 40px;}.footer-4 .w-social {display: flex;justify-content: space-between;}.footer-4 .btn .fa {font-size: 18px;color: #fff;}.footer-4 .btn {display: inline-block;text-align: center;flex-basis: 20%;}.btn-fb {border: 1px solid #3a589e !important;background: #3a589e !important;}.btn-tw {border: 1px solid #429cd6 !important;background: #429cd6 !important;}.btn-ig {border: 1px solid #bc2a8d !important;background: #bc2a8d !important;}.btn-gp {border: 1px solid #df4b37 !important;background: #df4b37 !important;}.btn-pi {border: 1px solid #cd2029 !important;background: #cd2029 !important;}.btn-in {border: 1px solid #0d77b7 !important;background: #0d77b7 !important;}.btn-yt {border: 1px solid #cd201f !important;background: #cd201f !important;}.postingan {padding: 40px;font-size: 14px }.postingan h2 {margin-bottom: 30px;font-size: 30px }img.recent-post-thumb {padding: 2px;width: 65px;height: 65px;float: left;margin: 0 10px 10px 0;border: 1px solid #f5f5f5 }.recent-posts-container {font-size: 12px }ul.recent-posts-container li {list-style-type: none;margin-bottom: 10px;font-size: 14px;float: left }ul.recent-posts-container li:before {display: none }ul.recent-posts-container {counter-reset: countposts;list-style-type: none;padding-left: 0!important }ul.recent-posts-container li:nth-child(3n+1) {padding-left: 0 }.recent-posts-container a {text-decoration: none }.recent-post-title {margin-bottom: 5px }.recent-post-title a {font-size: 14px;font-weight: bold;color: #2aace3 }.recent-posts-details {margin: 10px auto;font-size: 13px;color: #999 }.recent-posts-details a {color: #999 }.postingan2 {padding: 40px;}.postingan2 .wrap2 {padding: 0 10px;}.postingan2 .kolom13 {width: 33.33333333%;padding: 0;}.postingan2 h2 {font-size: 30px;margin-bottom: 30px;}.postingan2 img.recent-post-thumb {float: none;width: auto;height: auto;padding: 0;margin:0;border: none;}.postingan2 .thumb2 {height: 160px;overflow:hidden;margin-bottom: 10px;}.postingan3, .postingan4 {padding: 40px;background: #eee;}.postingan3 .wrap3,.postingan4 .wrap4 {margin:0px;text-align: center;background: #fff;padding:0px;}.postingan3 .kolom13 {width: 33.33333333%;padding: 0;}.postingan3 h2 {font-size: 30px;margin-bottom: 30px;}.postingan3 .recent-post-title {padding: 0 10px;}.postingan3 img.recent-post-thumb {float: none;width: auto;height: auto;padding: 0;margin:0;border: none;}.postingan3 .thumb3 {height: auto;overflow:hidden;margin-bottom: 10px;}.postingan3 .fa {font-size: 16px;}.postingan3 .masonry {-moz-column-count: 3;-webkit-column-count: 3;column-count: 3;margin: 1.5em 0;padding: 0;-moz-column-gap: 1.5em;-webkit-column-gap: 1.5em;column-gap: 1.5em;}.postingan3 .masonry-item {display: inline-block;background: #fff;padding: 0;margin: 0 0 1.5em;width: 100%;box-sizing: border-box;-moz-box-sizing: border-box;-webkit-box-sizing: border-box;box-shadow: 0px 1px 1px 0px rgba(0, 0, 0, 0.18);break-inside: avoid;}.postingan4 h2 {font-size: 30px;margin-bottom: 30px;}.postingan4 .recent-post-title {padding: 0 10px;}.postingan4 img.recent-post-thumb {float: none;width: auto;height: auto;padding: 0;margin:0;border: none;}.postingan4 .thumb4 {height: auto;overflow:hidden;margin-bottom: 10px;}.postingan4 .fa {font-size: 16px;}.postingan4 .masonry {-moz-column-count: 4;-webkit-column-count: 4;column-count: 4;margin: 1.5em 0;padding: 0;-moz-column-gap: 1.5em;-webkit-column-gap: 1.5em;column-gap: 1.5em;}.postingan4 .masonry-item {display: inline-block;background: #fff;padding: 0;margin: 0 0 1.5em;width: 100%;box-sizing: border-box;-moz-box-sizing: border-box;-webkit-box-sizing: border-box;box-shadow: 0px 1px 1px 0px rgba(0, 0, 0, 0.18);break-inside: avoid;}.postingan5 {padding: 40px 0px 0px;}.postingan5 h2 {margin-bottom: 30px;}.postingan5 .recent-post-title {padding: 0 10px;}.postingan5 img.recent-post-thumb {float: none;width: auto;height: auto;display: block;padding: 0;margin:0;border: none;}.postingan5 .thumb5 {height: auto;overflow:hidden;margin-bottom:0px;}.postingan5 .fa {font-size: 16px;}.postingan5 .masonry {-moz-column-count: 3;-webkit-column-count: 3;column-count: 3;margin: 1.5em 0;padding: 0;-moz-column-gap: 0em;-webkit-column-gap: 0em;column-gap: 0em;-webkit-flex-direction: row;flex-direction: row;}.postingan5 .masonry-item {display: inline-block;background: #fff;padding: 0;margin: 0;width: 100%;box-sizing: border-box;-moz-box-sizing: border-box;-webkit-box-sizing: border-box;box-shadow: 0px 1px 1px 0px rgba(0, 0, 0, 0.18);break-inside: avoid;transition: .8s opacity;}.postingan5 .masonry:hover .masonry-item {opacity:0.7;}.postingan5 .masonry:hover .masonry-item:hover {opacity: 1;}.bagikan {position: relative;display: block;overflow: hidden;margin: 25px 0 15px;padding: 15px 0;border-top: 1px dotted #f0f0f0;border-bottom: 1px dotted #f0f0f0 }.bagikan .fa {font-size: inherit;}.label-bagikan {display: block;float: left;height: 30px;line-height: 30px;margin: 8px 15px 8px 0;padding: 0 }.bagikan a {float: left;font-size: 12px;line-height: 30px;color: #fff;-webkit-border-radius: 2px;-moz-border-radius: 2px;border-radius: 2px;margin: 8px 3px;padding: 0 20px;height: 30px;min-width: 30px;text-align: center }.bagikan .facebook {background: #3b5998 }.bagikan .twitter {background: #0084b4 }.bagikan .googleplus {background: #d34836 }.bagikan .linkedin {background: #0077B5 }.bagikan .pinterest {background: #C92228 }.bagikan .whatsapp {background: #1c9b00;}mark {padding: 0 5px;}mark.merah {background: red;color: #fff;}mark.biru {background: blue;color: #fff;}mark.hijau {background: green;color: #fff;}mark.orange {background: orange;color: #fff;}.form-control {padding: 10px;height: 46px;border-radius: 5px;border: none;font-size: 16px;box-sizing: border-box;vertical-align: top;margin: 3px;}.btn {display: inline-block;padding: 10px 15px;margin: 3px;font-size: 16px;font-weight: 400;line-height: 1.42857143;text-align: center;white-space: nowrap;vertical-align: middle;-ms-touch-action: manipulation;touch-action: manipulation;cursor: pointer;-webkit-user-select: none;-moz-user-select: none;-ms-user-select: none;user-select: none;background: #fb9f00;border: 2px solid transparent;border-radius: 4px;}.btn:hover {opacity: .9 }.btn:active {position: relative;top: 1px }.btn-line {background-color: transparent;-moz-border-radius: 5px;-webkit-border-radius: 5px;border-radius: 5px;border: 2px solid #fb9f00;display: inline-block;cursor: pointer;color: #fb9f00!important;font-size: 16px;padding: 10px 15px;text-decoration: none;text-align: center;white-space: nowrap;vertical-align: middle }.btn-line:hover {background-color: transparent }.btn-line:active {position: relative;top: 1px }.btn-bulat {border-radius: 50px }.btn-besar {font-size: 25px;padding: 15px 30px;}.btn-super {-moz-box-shadow: 0px 10px 14px -7px #575757;-webkit-box-shadow: 0px 10px 14px -7px #575757;box-shadow: 0px 10px 14px -7px rgba(0, 0, 0, 0.5);background:-webkit-gradient(linear, left top, left bottom, color-stop(0.05, #f5a300), color-stop(1, #f58700));background:-moz-linear-gradient(top, #f5a300 5%, #f58700 100%);background:-webkit-linear-gradient(top, #f5a300 5%, #f58700 100%);background:-o-linear-gradient(top, #f5a300 5%, #f58700 100%);background:-ms-linear-gradient(top, #f5a300 5%, #f58700 100%);background:linear-gradient(to bottom, #f5a300 5%, #f58700 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#f5a300', endColorstr='#f58700',GradientType=0);background-color:#f5a300;-moz-border-radius:10px;-webkit-border-radius:10px;border-radius:10px;display:inline-block;cursor:pointer;color:#ffffff;font-size:30px;font-weight:bold;padding:20px 30px;line-height: 30px;}.btn-super:hover {background:-webkit-gradient(linear, left top, left bottom, color-stop(0.05, #f58700), color-stop(1, #f5a300));background:-moz-linear-gradient(top, #f58700 5%, #f5a300 100%);background:-webkit-linear-gradient(top, #f58700 5%, #f5a300 100%);background:-o-linear-gradient(top, #f58700 5%, #f5a300 100%);background:-ms-linear-gradient(top, #f58700 5%, #f5a300 100%);background:linear-gradient(to bottom, #f58700 5%, #f5a300 100%);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#f58700', endColorstr='#f5a300',GradientType=0);background-color:#f58700;text-decoration: none;}.btn-super:active {position:relative;top:1px;}.btn-super span {font-size: 20px;}.btn-merah {background: #CF000F;color: #fff !important;}.btn-pink {background: #DB0A5B;color: #333 !important;}.btn-hijau {background: #27ae60;color: #fff !important;}.btn-hijaumuda {background: #87D37C;color: #fff !important;}.btn-orange {background: #e67e22;color: #fff !important;}.btn-kuning {background: #ffde00;color: #333 !important;}.btn-ungu {background: #8e44ad;color: #fff !important;}.btn-ungumuda {background: #9B59B6;color: #fff !important;}.btn-biru {background: #446CB3;color: #fff !important;}.btn-birumuda {background: #19B5FE;color: #fff !important;}.btn-abu {background: #6C7A89;color: #fff !important;}.btn-putih {background: #fff;color: #111!important }.btn-hitam {background: #111;color: #fff !important;}.btn-line-merah {border: 2px solid #CF000F;color: #CF000F!important }.btn-line-pink {border: 2px solid #DB0A5B;color: #DB0A5B!important }.btn-line-hijau {border: 2px solid #27ae60;color: #27ae60!important }.btn-line-hijaumuda {border: 2px solid #87D37C;color: #87D37C!important }.btn-line-orange {border: 2px solid #e67e22;color: #e67e22!important }.btn-line-kuning {border: 2px solid #f1c40f;color: #f1c40f!important }.btn-line-ungu {border: 2px solid #8e44ad;color: #8e44ad!important }.btn-line-ungumuda {border: 2px solid #9B59B6;color: #9B59B6 !important }.btn-line-biru {border: 2px solid #446CB3;color: #446CB3!important }.btn-line-birumuda {border: 2px solid #19B5FE;color: #19B5FE!important }.btn-line-abu {border: 2px solid #6C7A89;color: #6C7A89!important }.btn-line-putih {border: 2px solid #fff;color: #fff!important }.btn-line-hitam {border: 2px solid #111;color: #111!important }.kotak {padding: 20px 20px;margin-bottom: 20px;background: #e7e7e7;border: solid 1px #e7e7e7;color: #666 }.kotak-merah {background: #e0b1b1;color: #ad4f4f;border: solid 1px #ad4f4f }.kotak-kuning {background: #fdf9d2;color: #af820a;border: solid 1px #d3cb6f }.kotak-biru {background: #C5EFF7;color: #3A539B;border: solid 1px #81CFE0 }.kotak-hijau {background: #C8F7C5;color: #049372;border: solid 1px #049372 }.box-konten ul.check, ul.check, ul.silang {list-style: none;padding-left: 15px;margin: 0 }.box-konten ul.check li:before, ul.check li:before {font-family: 'FontAwesome';content: '\f00c';margin: 0 10px 0 -26px;color: #25cd66 }.box-konten ul.silang li:before, ul.silang li:before {font-family: 'FontAwesome';content: '\f00d';margin: 0 10px 0 -26px;color: #cd2525 }.box-konten ul li,.box-konten ol li {margin-bottom: 15px;padding-left: 10px }.box-konten ul li ul {margin-top: 15px }ul.silang li ul, ul.check li ul {list-style: none }blockquote {font-style: italic }blockquote:before {font-family: 'FontAwesome';content: '\f10e';margin: 0 10px 0 -26px;color: #999 }blockquote.besar {font-size: 28px }blockquote.besar:before {font-family: 'FontAwesome';content: '\f10e';margin: 0 10px 0 -35px;color: #999 }.dropcap {font-size: 48px;font-weight: bold;float: left;display: block;margin: 0 7px 0 0;line-height: 1 }.breadcrumbs {font-size: 12px;border-bottom: solid 1px #fbfbfb;padding-top:30px; padding-bottom: 15px }.main-outer {border-top: $(main.border.width) solid $(body.rule.color) }.fauxcolumn-left-outer .fauxcolumn-inner {border-right: 1px solid $(body.rule.color) }.fauxcolumn-right-outer .fauxcolumn-inner {border-left: 1px solid $(body.rule.color) }div.widget > h2, div.widget h2.title {margin: 0 0 1em;font: $(widget.title.font);color: $(widget.title.text.color);border-bottom: solid 1px #FBFBFB;padding-bottom: 15px }.widget .zippy {color: $(widget.alternate.text.color);text-shadow: 2px 2px 1px rgba(0, 0, 0, .1) }.widget .popular-posts ul {list-style: none }h2.date-header {font: $(date.header.font) }.date-header span {background-color: $(date.header.background.color);color: $(date.header.color);padding: $(date.header.padding);letter-spacing: $(date.header.letterspacing);margin: $(date.header.margin) }.main-inner {padding-top: $(main.padding.top);padding-bottom: $(main.padding.bottom) }.main-inner .column-center-inner {padding: 0 $(main.padding) }.main-inner .column-center-inner .section {margin: 0 $(main.section.margin) }.xopostimg {max-width: 100px;float: left;margin: 0 30px 15px 0 !important;}.xopostsummary {display: inline }.post {margin: 0 0 $(post.margin.bottom) }h2.post-title {font: $(post.title.font);color: #222;margin: 0;margin-bottom: .125em;padding: 0;line-height: 1.15em;letter-spacing: -.0625em }h2.post-title a {color: #222 }.post-body {font-size: 100%;line-height: 1.4;position: relative }.post-body img, .post-body .tr-caption-container, .Profile img, .Image img, .BlogList .item-thumbnail img {padding: $(image.border.small.size);background: $(image.background.color); }.post-body img, .post-body .tr-caption-container {padding: $(image.border.large.size) }.post-body .tr-caption-container {color: $(image.text.color) }.post-body .tr-caption-container img {padding: 0;background: transparent;border: none;-moz-box-shadow: 0 0 0 rgba(0, 0, 0, .1);-webkit-box-shadow: 0 0 0 rgba(0, 0, 0, .1);box-shadow: 0 0 0 rgba(0, 0, 0, .1) }.post-header {margin: .7em 0 1.5em;line-height: 1.6;font-size: 12px;color: #222 }.post-header a {color: #222 }.post-footer {font-size: 12px;margin: 20px auto;padding: 0;color: $(post.footer.text.color);background-color: $(post.footer.background.color);border-bottom: 1px solid $(post.footer.border.color);line-height: 1.6 }.post-timestamp {margin-left: 0 }#comments .comment-author {padding-top: 1.5em;border-top: 1px solid $(body.rule.color);background-position: 0 1.5em }#comments .comment-author:first-child {padding-top: 0;border-top: none }.avatar-image-container {margin: .2em 0 0 }#comments .avatar-image-container img {border: 1px solid $(image.border.color) }.sidebar .widget-content {color: #333;font-size: 14px }.jump-link {margin-top: 15px }.jump-link a {color: #333;padding: 5px 10px;background: #fbfbfb }.comments .comments-content .icon.blog-author {background-repeat: no-repeat;background-image: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAYAAABWzo5XAAAAAXNSR0IArs4c6QAAAAZiS0dEAP8A/wD/oL2nkwAAAAlwSFlzAAALEgAACxIB0t1+/AAAAAd0SU1FB9sLFwMeCjjhcOMAAAD+SURBVDjLtZSvTgNBEIe/WRRnm3U8RC1neQdsm1zSBIU9VVF1FkUguQQsD9ITmD7ECZIJSE4OZo9stoVjC/zc7ky+zH9hXwVwDpTAWWLrgS3QAe8AZgaAJI5zYAmc8r0G4AHYHQKVwII8PZrZFsBFkeRCABYiMh9BRUhnSkPTNCtVXYXURi1FpBDgArj8QU1eVXUzfnjv7yP7kwu1mYrkWlU33vs1QNu2qU8pwN0UpKoqokjWwCztrMuBhEhmh8bD5UDqur75asbcX0BGUB9/HAMB+r32hznJgXy2v0sGLBcyAJ1EK3LFcbo1s91JeLwAbwGYu7TP/3ZGfnXYPgAVNngtqatUNgAAAABJRU5ErkJggg==) }.comments .comments-content .loadmore a {border-top: 1px solid $(widget.alternate.text.color);border-bottom: 1px solid $(widget.alternate.text.color) }.comments .comment-thread.inline-thread {background-color: $(post.footer.background.color) }.comments .continue {border-top: 2px solid $(widget.alternate.text.color) }.section-columns td.columns-cell {border-startside: 1px solid $(body.rule.color) }.blog-pager {background: $(paging.background);overflow: visible!important }.topnav .icon .fa, .blog-pager .fa {font-size: inherit;}.blog-pager-older-link, .home-link, .blog-pager-newer-link {background-color: $(content.background.color);padding: 0 }.blog-pager span {margin: 0 2px;background: #fbfbfb;padding: 5px 10px }#blog-pager-newer-link span, #blog-pager-older-link span {background: none;padding: 0;margin: 0 }.footer-outer {border-top: $(footer.bevel) dashed #bbbbbb }.footer-inner {padding: 0 }ul.topnav li.icon {display: none }ul.topnav li.icon a {background: #293003;color: #fff }#blog-pager-newer-link {text-align: left;width: 40% }#blog-pager-older-link {text-align: right;width: 40% }#blog-pager-older-link h6 {margin: 0;padding: 0;text-align: right;font-family: &#39;font-size: 14px;color: #333333;text-transform: uppercase;line-height: 1.625em;font-weight: 700 }#blog-pager-newer-link h6 {margin: 0;padding: 0;text-align: left;font-family: &#39;font-size: 14px;color: #;text-transform: uppercase;line-height: 1.625em;font-weight: 700 }.pager-content {width: 99.5%;overflow: hidden;margin: 10px 0 0;padding: 10px 0 0 }.pager-content a:hover, .pager-content {color: #000;text-decoration: none }.showpageNum a, .showpage a, .showpagePoint {background: #DE3C3C;color: #FFF;font-size: 15px;font-family: open sans;font-weight: 700;margin-left: 10px;margin-right: 10px;border-radius: 5px 5px 5px 5px;-webkit-border-radius: 5px 5px 5px 5px;-moz-border-radius: 5px;-o-border-radius: 5px 5px 5px 5px;transition: background 400ms;-webkit-transition: background 400ms;-moz-transition: background 400ms;-o-transition: background 400ms;padding: 10px 20px }.showpageNum a:hover, .showpage a:hover, .showpagePoint, .blog-pager-newer-link, .blog-pager-older-link, .home-link {color: #FFF }.box-konten .ContactForm {padding: 40px;background: url(https://4.bp.blogspot.com/-7XtveurYgOs/WOjE2Z6HoVI/AAAAAAAAAcU/lrxX3uDvcTAP9lJSSnbOXEE4VSpY4GNbgCLcB/s1600/contact-bg.png) no-repeat; background-size: cover;}.box-konten .ContactForm .contact-form-widget {background: #fff;padding: 5px 20px;}.box-konten .ContactForm {text-align:center;}.box-konten .ContactForm h2.title {max-width: 250px;background: #e74c3c;color: #fff;padding: 15px 20px;margin: auto !important;font-size: 20px !important;}.box-konten .ContactForm .contact-form-widget {margin: auto;font-size: 12px;}.box-konten .ContactForm .contact-form-widget form input, .box-konten .ContactForm .contact-form-widget form textarea {padding: 15px 10px;border-radius: 5px;}.box-konten .ContactForm .contact-form-widget form input.contact-form-button {line-height: normal;height: auto;font-size: 14px;width: 220px;padding: 10px;20px;background: #e74c3c;border: none;}.box-konten .ContactForm .contact-form-widget form div:last-child {margin: auto;}.showpageOf {display: none!important }iframe.blogger-iframe-colorize, iframe.blogger-comment-from-post {height: 210px!important }iframe {width: 100% }.copy {text-align: center;font-size: 12px;padding-top: 20px;padding-bottom: 20px;color: #999 }.sl-wrapper .sl-close,.sl-wrapper .sl-navigation button{height:44px;line-height:44px;font-family:Arial,Baskerville,monospace}body.hidden-scroll{overflow:hidden}.sl-overlay{position:fixed;left:0;right:0;top:0;bottom:0;background:#000;opacity:.9;display:none;z-index:1050}.sl-wrapper .sl-close,.sl-wrapper .sl-counter{top:30px;display:none;color:#fff;position:fixed}.sl-wrapper{z-index:1040}.sl-wrapper button{border:0;background:0 0;font-size:28px;padding:0;cursor:pointer}.sl-wrapper button:hover{opacity:.7}.sl-wrapper .sl-close{right:30px;z-index:1060;margin-top:-14px;margin-right:-14px;width:44px;font-size:3rem}.sl-wrapper .sl-counter{left:30px;z-index:1060;font-size:1rem}.sl-wrapper .sl-navigation{width:100%;display:none}.sl-wrapper .sl-navigation button{position:fixed;top:50%;margin-top:-22px;width:22px;text-align:center;display:block;z-index:1060;color:#fff}.sl-wrapper .sl-navigation button.sl-next{right:5px;font-size:2rem}.sl-wrapper .sl-navigation button.sl-prev{left:5px;font-size:2rem}.sl-wrapper .sl-image{position:fixed;-ms-touch-action:none;touch-action:none;z-index:10000}.sl-wrapper .sl-image img{margin:0;padding:0;display:block;border:0}.sl-wrapper .sl-image iframe{background:#000;border:0}@media (min-width:35.5em){.sl-wrapper .sl-navigation button{width:44px}.sl-wrapper .sl-navigation button.sl-next{right:10px;font-size:3rem}.sl-wrapper .sl-navigation button.sl-prev{left:10px;font-size:3rem}.sl-wrapper .sl-image iframe,.sl-wrapper .sl-image img{border:0}}@media (min-width:50em){.sl-wrapper .sl-navigation button{width:44px}.sl-wrapper .sl-navigation button.sl-next{right:20px;font-size:3rem}.sl-wrapper .sl-navigation button.sl-prev{left:20px;font-size:3rem}.sl-wrapper .sl-image iframe,.sl-wrapper .sl-image img{border:0}}.sl-wrapper .sl-image .sl-caption{display:none;padding:10px;color:#fff;background:rgba(0,0,0,.8);position:absolute;bottom:0;left:0;right:0}.sl-wrapper .sl-image .sl-caption.pos-top{bottom:auto;top:0}.sl-wrapper .sl-image .sl-caption.pos-outside{bottom:auto}.sl-wrapper .sl-image .sl-download{display:none;position:absolute;bottom:5px;right:5px;color:#000;z-index:1060}.sl-spinner{display:none;border:5px solid #333;border-radius:40px;height:40px;left:50%;margin:-20px 0 0 -20px;opacity:0;position:fixed;top:50%;width:40px;z-index:1007;-webkit-animation:pulsate 1s ease-out infinite;-moz-animation:pulsate 1s ease-out infinite;-ms-animation:pulsate 1s ease-out infinite;-o-animation:pulsate 1s ease-out infinite;animation:pulsate 1s ease-out infinite}.sl-scrollbar-measure{position:absolute;top:-9999px;width:50px;height:50px;overflow:scroll}@-webkit-keyframes pulsate{0%{transform:scale(.1);opacity:0}50%{opacity:1}100%{transform:scale(1.2);opacity:0}}@keyframes pulsate{0%{transform:scale(.1);opacity:0}50%{opacity:1}100%{transform:scale(1.2);opacity:0}}@-moz-keyframes pulsate{0%{transform:scale(.1);opacity:0}50%{opacity:1}100%{transform:scale(1.2);opacity:0}}@-o-keyframes pulsate{0%{transform:scale(.1);opacity:0}50%{opacity:1}100%{transform:scale(1.2);opacity:0}}@-ms-keyframes pulsate{0%,100%{opacity:0}0%{transform:scale(.1)}50%{opacity:1}100%{transform:scale(1.2)}}.slick-list,.slick-slider,.slick-track{position:relative;display:block}.slick-loading .slick-slide,.slick-loading .slick-track{visibility:hidden}.slick-slider{-moz-box-sizing:border-box;box-sizing:border-box;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;-webkit-touch-callout:none;-khtml-user-select:none;-ms-touch-action:pan-y;touch-action:pan-y;-webkit-tap-highlight-color:transparent}.slick-list{overflow:hidden;margin:0;padding:0}.slick-list:focus{outline:0}.slick-list.dragging{cursor:pointer;cursor:hand}.slick-slider .slick-list,.slick-slider .slick-track{-webkit-transform:translate3d(0,0,0);-moz-transform:translate3d(0,0,0);-ms-transform:translate3d(0,0,0);-o-transform:translate3d(0,0,0);transform:translate3d(0,0,0);padding: 20px 0px;}.slick-track{top:0;left:0}.slick-track:after,.slick-track:before{display:table;content:''}.slick-track:after{clear:both}.slick-slide{display:none;float:left;height:100%;min-height:1px}[dir=rtl] .slick-slide{float:right}.slick-slide img{display:block}.slick-slide.slick-loading img{display:none}.slick-slide.dragging img{pointer-events:none}.slick-initialized .slick-slide{display:block}.slick-vertical .slick-slide{display:block;height:auto;border:1px solid transparent}.slick-arrow.slick-hidden{display:none}.screenshot-slider img {opacity:0.3;margin: auto;transition:all 300ms ease;}.screenshot-slider .slick-center img{-moz-transform:scale(1.08);-ms-transform:scale(1.08);-o-transform:scale(1.08);-webkit-transform:scale(1.08);opacity:1;transform:scale(1.08);}.slick-prev, .slick-next {font-size: 0;line-height: 0;position: absolute;top: 50%;display: block;width: 20px;height: 20px;margin-top: -10px;padding: 0;cursor: pointer;color: transparent;border: none;outline: none;background: transparent;}.slick-prev:hover, .slick-prev:focus, .slick-next:hover, .slick-next:focus {color: transparent;outline: none;background: transparent;}.slick-prev:hover:before, .slick-prev:focus:before, .slick-next:hover:before, .slick-next:focus:before {opacity: 1;}.slick-prev.slick-disabled:before, .slick-next.slick-disabled:before {opacity: .25;}.slick-prev:before, .slick-next:before {font-family: FontAwesome;font-size: 20px;line-height: 1;opacity: .75;color: #999;-webkit-font-smoothing: antialiased;-moz-osx-font-smoothing: grayscale;}.slick-prev {left: -25px;}[dir='rtl'] .slick-prev {right: -25px;left: auto;}.slick-prev:before {content: "\f137";}[dir='rtl'] .slick-prev:before {content: "\f137";}.slick-next {right: -25px;}[dir='rtl'] .slick-next {right: auto;left: -25px;}.slick-next:before {content: "\f138";}[dir='rtl'] .slick-next:before {content: "\f138";}.slick-slider {margin-bottom: 30px;}.slick-dots {position: absolute;bottom: -45px;display: block;width: 100%;padding: 0;list-style: none;text-align: center;}.slick-dots li {position: relative;display: inline-block;width: 20px;height: 20px;margin: 0 5px;padding: 0;cursor: pointer;}.slick-dots li button {font-size: 0;line-height: 0;display: block;width: 20px;height: 20px;padding: 5px;cursor: pointer;color: transparent;border: 0;outline: none;background: transparent;}.slick-dots li button:hover, .slick-dots li button:focus {outline: none;}.slick-dots li button:hover:before, .slick-dots li button:focus:before {opacity: 1;}.slick-dots li button:before {font-family: 'slick';font-size: 6px;line-height: 20px;position: absolute;top: 0;left: 0;width: 20px;height: 20px;content: 'â€¢';text-align: center;opacity: .25;color: black;-webkit-font-smoothing: antialiased;-moz-osx-font-smoothing: grayscale;}.slick-dots li.slick-active button:before {opacity: .75;color: black;}.ngambang {position: fixed !important;z-index: 999999;left: 20px !important;right: auto;top: 20px !important;height: 130px !important;width: 250px !important;padding: 5px;border-radius: 4px;background: #fff;box-shadow: 0 5px 10px rgba(0,0,0,0.2);}.show {display: block;}.hide {display: none;}#related-posts .row {display: grid;grid-template-columns: auto auto auto;grid-column-gap: 5px;grid-row-gap: 5px;width: 100%;}#related-posts .row .col:first-child{margin: 0 auto;}#related-posts .row .col{margin: 0 auto;}#related-posts .related_img {margin:5px;object-fit: cover;height: 145px;-webkit-border-radius: 5px;-moz-border-radius: 5px;border-radius: 5px;}#related-title {color:#333;text-transform:capitalize;padding: 0px 5px 10px;font-size:14px;}/* ++++++++++++ RESPONSIVE LAYOUT +++++++++++ *//* ++++++++++ AROODAM LANDING PAGE ++++++++++ *//* ++++++++++++++++++++++++++++++++++++++++++ */@media only screen and (min-width: 768px) and (max-width: 959px) {body {min-width: 767px;padding: 0!important }}@media only screen and (max-width: 767px) {body {min-width: 320px;padding: 0!important }.box-konten h2, .box-pricing h2 {font-size: 30px !important;margin-bottom: 15px;}.btn-besar {font-size: 16px;}p.txt-caption {font-size: 16px;}.Header h1 {font-size: 25px }.Header .description {font-size: 16px }ul.topnav li:not(:first-child) {display: none }ul.topnav li.icon {float: right;display: inline-block }ul.topnav.responsive {position: relative }ul.topnav.responsive li.icon {position: absolute;right: 0;top: 0 }ul.topnav.responsive li {float: none;display: inline }ul.topnav.responsive li a {display: block;text-align: left }.pad40 {padding: 30px 15px }.cover h1, .cover h2 {font-size: 24px;margin: 0 0 20px }.cover p {font-size: 16px;margin: 0 0 20px }.cover1 {padding: 30px 15px }.cover2 {padding: 30px 15px;text-align: center }.cover3 {padding: 60px 15px }.cover4 {padding: 50px 15px;text-align: center }.cover5 {padding: 20px 15px }.cover5 li {font-size: 16px;margin-bottom: 5px }.cover6 {text-align: center;margin: 30px 15px;padding: 0 }.cover7, .cover8,.cover9,.cover10, .cover11 {padding: 30px 15px;}.cover9 {text-align:center;}.cover9 .isi {padding-top: 0;padding-left: 0;}.cover10 .waktu {font-size: 13px;}.cover10 .waktu span {font-size: 2em;}.cover11 {padding-left: 15px;padding-right: 15px;padding-top: 50px;padding-bottom: 50px;}.cover11 .btn {display: inline;}.cover12 .full-row {left: 15%;transform: translate(-9%,-50%);}.cover12 {height: 50vh;}.isi-konten {padding: 3em 15px }.feat-1, .feat-2, .feat-3, .feat-4, .feat-5, .feat-6, .feat-7, .feat-8, .feat-9, .feat-11, .feat-12, .feat-13, .feat-14, .feat-15, .feat-16, .feat-17, .feat-18, .feat-19, .feat-20, .feat-21, .feat-22, .feat-23 {padding: 20px 15px;}.feat-2 .col {text-align: left;}.feat-2 .col .list-box {padding: 0 }.feat-10 .feat-list {width: 100%;}.feat-10 .feat-list .padding{padding:15px;}.feat-20 .btn {margin-left: 0 }.feat-11 .wrap-video , .feat-13 .wrap-video {height: 250px;}.feat-24 h2 span {display: block;margin: 20px auto;}.feat-26, .feat-27, .feat-28, .feat-29 {padding: 30px 15px;}.feat-30 .row .col {width: 100%;}.feat-30 .row{display: -webkit-flex;display: -ms-flexbox;display: flex;flex-direction: column;}.feat-30 .row .col {flex:1 0 50%;box-sizing: border-box;}.feat-31 {padding: 30px 15px;}.feat-32 .head-feat {padding: 30px 15px;}.feat-32 .gkanan {padding-top: 10px;}.feat-32 .feat-list .col.gkanan img {position: relative;right: 0;bottom:0;width: 70%;}.feat-33 .head-feat {padding: 30px 15px;}.feat-33 .gkiri {padding-top: 10px;}.feat-33 .feat-list .col.gkiri img {position: relative;left: 0;bottom:0;width: 70%;}.feat-34 {padding: 30px 15px 0 15px;}.feat-34 .col {margin-bottom: 0;}.feat-35 {padding: 30px 15px;}.feat-35 .col:first-child {text-align: center;margin-top: 0px;}.feat-35 .col:last-child {text-align: center;margin-top: 0px;}.feat-36 {padding: 30px 15px;}.feat-36 .video-slider iframe {height: 300px;}.feat-37 {padding: 30px 15px 0px 15px;}.feat-37 .gbawah {padding-top: 10px;}.feat-37 .feat-list .col.gbawah img {position: relative;right: 0;bottom:0;width: 90%;}.feat-38,.feat-39 {padding: 30px 15px;}.feat-39 .row .col:nth-child(2) .step {padding: 50px 0px;}.feat-39 .row .col:nth-child(2) .step:before {-webkit-transform: rotate(90deg);-moz-transform: rotate(90deg);-ms-transform: rotate(90deg);-o-transform: rotate(90deg);transform: rotate(90deg);left: 47.5%;top: -4%;}.feat-39 .row .col:nth-child(2) .step:after {-webkit-transform: rotate(90deg);-moz-transform: rotate(90deg);-ms-transform: rotate(90deg);-o-transform: rotate(90deg);transform: rotate(90deg);right: 47.5%;bottom: 4%;}.feat-39 .row .col {width: 100%;}.feat-40 .row .col:nth-child(3n+2) .step {padding: 50px 0px;}.feat-40 .row .col:nth-child(3) .step {padding-bottom: 50px;}.feat-40 .row .col:nth-child(3) .step:after {background: url("https://2.bp.blogspot.com/-hBqikdXy3Kk/WPK2muNQwoI/AAAAAAAAAg0/K8TkndIAgB8WaHZEvLQnskAd_fPLLAjMwCLcB/s1600/step-icon.png") no-repeat ;-webkit-transform: rotate(90deg);-moz-transform: rotate(90deg);-ms-transform: rotate(90deg);-o-transform: rotate(90deg);transform: rotate(90deg);left: 47.5%;bottom: 0px;}.feat-40 .row .col:nth-child(3n+2) .step:before {-webkit-transform: rotate(90deg);-moz-transform: rotate(90deg);-ms-transform: rotate(90deg);-o-transform: rotate(90deg);transform: rotate(90deg);left: 47.5%;top: -6%;}.feat-40 .row .col:nth-child(3n+2) .step:after {-webkit-transform: rotate(90deg);-moz-transform: rotate(90deg);-ms-transform: rotate(90deg);-o-transform: rotate(90deg);transform: rotate(90deg);right: 47.5%;bottom: 0px;}.feat-40 .row .col, .feat-41 .row .col {width: 100%;}.feat-41 .row{display: -webkit-flex;display: -ms-flexbox;display: flex;flex-direction: column;}.feat-41 .row .col {flex:1 0 50%;box-sizing: border-box;}.feat-42 .row .col {width: 100%;}.feat-42 .row{display: -webkit-flex;display: -ms-flexbox;display: flex;flex-direction: column;}.feat-42 .row .col {flex:1 0 50%;box-sizing: border-box;}.feat-42 .row.tukar .col:first-child {margin-left: auto;order: 0;}.feat-43 {padding: 30px 15px;}.timeline:before {border-right: solid 2px #ffcf26;}.timeline span.date {font-size: 0.7em;}.timeline h3 {font-size: 18px;}ul.konten-tabs li, ul.v-tabs li {display: block;}.v-content {padding: 20px 0;}.v-content.current {border: none;border-top: solid 2px #3498db;}.pricing-1, .pricing-2 {padding: 20px 15px }.pricing-2 .table-harga-1 {padding-left: 0;padding-right: 0 }.pricing-3,.pricing-4,.pricing-5 {padding: 30px 15px }.tabel-harga {}.tabel-harga thead th:first-child {display:none;}.tabel-harga thead .sembunyi, .tabel-harga tbody .sembunyi {display: none;}.tampilkan ul.plan-tabs {display: table;}.cta-1, .cta-2, .cta-3,.cta-12,.cta-14,.cta-15,.cta-16 {padding: 30px 15px }.cta-1 .kotak-promo {width: 100% }.cta-1 .kotak-promo .harga-asli {float: none;margin: auto }.cta-1 .kotak-promo .harga-baru {width: 100% }.cta-1 .btn, .cta-2 .btn, .cta-3 .btn {font-size: 20px!important }.cta-5,.cta-6,.cta-7,.cta-8,.cta-9,.cta-11 {padding: 30px 15px }.cta-5 .form-subscribe fieldset, .cta-6 .form-subscribe fieldset {box-sizing: border-box;width: 100% }.cta-5 .form-subscribe fieldset .form-group, .cta-6 .form-subscribe fieldset .form-group {float: none }.cta-5 .form-subscribe fieldset .form-group .input-md, .cta-6 .form-subscribe fieldset .form-group .input-md {width: 100%;box-sizing: border-box;margin: 5px auto }.cta-5 .form-subscribe fieldset .form-group button, .cta-6 .form-subscribe fieldset .form-group button {width: 100%;box-sizing: border-box;margin: 5px auto }.cta-9 .order img {width: 30px;}.cta-12 .waktu,.cta-14 .waktu,.cta-15 .waktu {font-size: 11px;}.cta-12 .waktu span,.cta-14 .waktu span,.cta-15 .waktu span {font-size: 2em;}.cta-17 .btn span {display: none;}.btn-super {white-space: normal;}#slidebox {width: 100%;height: auto;}.testimoni-1 {padding: 30px 15px }.testimoni-2 {padding: 30px 15px 10px }.testimoni-4 {padding: 30px 14px;text-align: center;}.testimoni-4 .kolom-besar .isi-testi {margin-top: 0 }.testimoni-4 .ava {width: 200px;height: 200px }.testimoni-4 .tukar .isi-testi:after, .testimoni-4 .isi-testi:after {left: 50% }.testimoni-4 .tukar {text-align: center }.testimoni-5 {padding: 30px 15px;}.testimoni-7 {padding: 30px 14px;text-align: center;}.testimoni-7 .kolom-besar .isi-testi {margin-top: 0 }.testimoni-7 .ava {width: 200px;height: 200px }.testimoni-7 .tukar .isi-testi:after, .testimoni-7 .isi-testi:after {left: 50% }.testimoni-7 .tukar {text-align: center }.team-1, .team-2, .team-3, .team-4 {padding: 30px 15px }.postingan, .postingan2, .postingan3, .postingan4 {padding: 30px 15px }.postingan ul li {margin: 0;padding-left: 0 }.postingan2 .kolom13 {width: 100%;padding: 0;}.postingan3 .masonry, .postingan4 .masonry {-moz-column-count: 1;-webkit-column-count: 1;column-count: 1;}.faq-1, .faq-2, .faq-3, .footer-1, .footer-2, .footer-3 {padding: 30px 15px }.my-slider {margin: 0 15px }.unslider-wrap.unslider-carousel li {font-size: 12px }.content-inner {padding: 15px }.tabs-inner {padding: 0 }.main-inner .columns {padding-right: 0!important }.main-inner .column-center-inner {padding: 0px !important }.main-inner .column-center-inner .section {margin: 0!important }.column-center-outer {margin-bottom: 30px }.column-right-outer {clear: both;width: 100%!important }.column-right-inner {padding: 0!important }.section {margin: 0 !important }.modalDialog > div {max-width: 90%;}.box-konten .ContactForm {padding: 30px 15px;}.box-konten .ContactForm .contact-form-widget {}.form-control {width: 100%;}.btn {width: auto;}}
]]></b:skin>
    <b:template-skin>
      <b:variable default='960px' name='content.width' type='length' value='960px'/>
      <b:variable default='0' name='main.column.left.width' type='length' value='0px'/>
      <b:variable default='310px' name='main.column.right.width' type='length' value='0px'/>
      <![CDATA[
        body {} #Header1 img {padding: 20px 0;} #Header2 img {padding: 7px 0px;}.full .box-konten .row, .full .box-konten .head-feat {max-width: 100%;width: $(content.width);margin: 0 auto !important;}.region-inner {/*max-width: $(content.width) !important;*/}.content-outer, .content-fauxcolumn-outer {max-width: $(content.width);_width: $(content.width);}.main-inner .columns {padding-left: $(main.column.left.width);padding-right: $(main.column.right.width);}.main-inner .fauxcolumn-center-outer {left: $(main.column.left.width);right: $(main.column.right.width);_width: expression(this.parentNode.offsetWidth - parseInt("$(main.column.left.width)") - parseInt("$(main.column.right.width)") + 'px');}.main-inner .fauxcolumn-left-outer {width: $(main.column.left.width);}.main-inner .fauxcolumn-right-outer {width: $(main.column.right.width);}.main-inner .column-left-outer {width: $(main.column.left.width);right: 100%;margin-left: -$(main.column.left.width);}.main-inner .column-right-outer {width: $(main.column.right.width);margin-right: -$(main.column.right.width);}
.breadcrumbs {max-width: $(content.width);_width: $(content.width);margin: 0 auto !important;}
footer .footer-outer {max-width: $(content.width);_width: $(content.width);margin: 0 auto !important; padding-bottom: 30px;}
.column-right-inner {padding-top: 30px !important; }
body#layout .columns {padding-right: 250px;}
.sidebar.section {margin: 0 15px !important;}
footer .columns-cell {padding: 5px;}
        #layout {min-width: 0;background: none !important;border: none !important;}#layout:before {width: 80px;content: " ";background-image: url(https://1.bp.blogspot.com/-OPKCdc5TJbs/W55UgkGCLaI/AAAAAAAABCU/VkVmwuBdasMQ0HVoySpMvB0wdo_1ktyiwCLcBGAs/s1600/aroodam-2018.jpg);position: absolute;right: 25px;top: 2px;height: 80px;}#layout:after {font-family: arial;width: 355px;content: "Ikuti kami di Telegram/IG : @aroodam | WA : 085232355460" !important;position: absolute;right: 150px;top: 35px;height: 80px;visibility: visible !important;}#layout .header, #layout .header .widget-content {background: #d7d4ad !important;}#layout .tabs, #layout .tabs .widget-content {background: #88f2f1 !important;}#layout .w-cover, #layout .w-cover .widget-content {background: #e2a0a0 !important;}#layout #Pemisah1, #layout #Pemisah1 .widget-content {background: #b1b9de !important;}#layout #Features, #layout #Features .widget-content {background: #9accc6 !important;}#layout #Pemisah2, #layout #Pemisah2 .widget-content {background: #bfe2a0 !important;}#layout #Testimoni, #layout #Testimoni .widget-content {background: #bca0e2 !important;}#layout #Pemisah3, #layout #Pemisah3 .widget-content{background: #fef2af !important;}#layout #CallToAction, #layout #CallToAction .widget-content {background: #f3b7ef !important;}#layout #Pemisah4, #layout #Pemisah4 .widget-content{background: #94d195 !important;}#layout #Footer, #layout #Footer .widget-content {background: #f17d7d !important;}#layout .content-inner, .content-inner {padding: 0px !important;}#layout .column-center-inner {padding: 0px 0px 0px 4px !important;}#layout .content-outer {min-width: 0;width: 800px; margin: 0;}#layout .region-inner {min-width: 0;width: auto;padding: 0px;}body#layout div.add_widget {padding: 8px;}body#layout #navbar{max-width: 760px !important; margin: 8px 0;}body#layout div.section {border: 0px !important; margin: 5px 0;}body#layout .tabs-inner {padding: 0px;}body#layout div.add_widget a {margin-left: 32px;}
        body#layout .wrap-hm {overflow: hidden; padding-top: 35px;}
        body#layout .wrap-hm:before {
					font-family: arial;
					width: 100%;
					content: "Hapus Gadget jika tidak ingin menggunakan Header dan Menu di bawah ini" !important;
					white-space: pre;
					position: absolute;
					left: 3px; top: 10px;
					text-align: left;
					visibility: visible !important;
				}

        body#layout .kolom13 {width: 40%; display: block;float: left;}
        body#layout .kolom23 {width: 60%; display: block;float: left;}

        .tabs-inner .section,.wrap-hm, .cover .row, .aroodam-content-1 .row, .aroodam-content-2 .row, .aroodam-content-3 .row, .aroodam-content-4 .row, .aroodam-content-5 .row, .aroodam-content-6 .row, .aroodam-content-7 .row, .aroodam-content-8 .row {max-width: $(content.width);_width: $(content.width);margin: auto;}/* aroodam landing page 2.2 */.full .main-inner .row {max-width: 100%; margin: 0 auto !important;}.main-inner {padding-top: 0px;}.main-inner .head-feat h2,.main-inner .group h2 {margin-bottom: 15px;font-size: 48px;padding: 0;line-height: 1em;letter-spacing: -.0625em;}.main-inner .head-feat h2 span, .main-inner .group h2 span {font-family: playfair display;font-style: italic;font-weight: bold;}.main-inner .group {margin: auto !important;}.main-inner .group p {margin-top: 10px; margin-bottom: 15px;}.main-inner .group .ava {margin: 20px auto !important;}.main-inner .group img {padding: 0px !important; background: transparent;}.main-inner .feat-32 .feat-list .col, .main-inner .feat-33 .feat-list .col {padding-bottom: 0; margin-bottom: 0;}.main-inner ul.price {padding: 0px !important;} #Header2 #header-inner {padding-top: 15px; padding-bottom: 15px;}.wrap-hm {position: relative;top: 50%;}.menunya {position: relative;} #crosscol1 {margin-top: 30px;}.menunya ul.topnav {float: right;}
        @media only screen and (max-width: 767px){
        .post-body .row.artikel, .post-footer, .comments, .breadcrumbs, .post-header, .post-title, #related-posts {width: auto;padding-left: 15px !important;padding-right: 15px !important;}
        .wrap-hm .col {margin:0px;}
        .wrap-hm .headernya {text-align: center;}
        .header-menu {padding-bottom: 0px;}
        #crosscol1 {margin-top: 0px;}
        .menunya ul.topnav {float: none;}
        .copy {font-size:7px;}
        }
        ]]>
    </b:template-skin>

    <!-- kondisi untuk menghilangkan postingan dan sidebar di halaman utama -->
    <b:if cond='data:blog.url != data:blog.homepageUrl'>
      <style>
          .content-inner {display: block;}
      </style>
    <b:else/>
      <style>
          .content-inner {display: none;}
      </style>
    </b:if>
    <!-- end kondisi -->

    <!-- PAGES LANDING PAGE (menghilangkan judul halaman) -->
    <b:if cond='data:blog.pageType == &quot;static_page&quot;'>
        <style>
            .breadcrumbs, .post-title, .post-header {display: none;}
        </style>
    </b:if>



    <b:if cond='data:skin.vars.body_background.image.isResizable and data:features.responsiveBackgrounds'>
      <b:include cond='not data:view.isPreview' data='{                          image: data:skin.vars.body_background.image,                          selector: &quot;body&quot;                        }' name='responsiveImageStyle'/>
    </b:if>
    <b:include data='blog' name='google-analytics'/>
    <script type='text/javascript'>
        var thumbnail_mode = &quot;yes&quot;;
        summary_noimg = 300;
        summary_img = 300;
        img_thumb_height = 100;
        img_thumb_width = 100;
    </script>
    <script type='text/javascript'>
        //<![CDATA[
        function removeHtmlTag(strx,chop){
            if(strx.indexOf("<")!=-1){
                var s = strx.split("<");
                for(var i=0;i<s.length;i++){
                    if(s[i].indexOf(">")!=-1){
                        s[i] = s[i].substring(s[i].indexOf(">")+1,s[i].length);
                    }
                }
            strx = s.join("");
            }

            chop = (chop < strx.length-1) ? chop : strx.length-2;

            while(strx.charAt(chop-1)!=' ' && strx.indexOf(' ',chop)!=-1) chop++;
            strx = strx.substring(0,chop-1);
            return strx+'...';
        }

        function createSummaryAndThumb(pID){
            var div = document.getElementById(pID);
            var imgtag = "";
            var img = div.getElementsByTagName("img");
            var summ = summary_noimg;
            if(img.length>=1) {
                imgtag = '<div class="xopostimg"><img src="'+img[0].src+'" width="100%" alt=""/></div>';
                summ = summary_img;
            }
            var summary = imgtag + '<div class="xopostsummary">' + removeHtmlTag(div.innerHTML,summ) + '</div>';
            div.innerHTML = summary;
        }
        function removeHtmlTag(strx,chop){if(strx.indexOf("<")!=-1){var s=strx.split("<");for(var i=0;i<s.length;i++){if(s[i].indexOf(">")!=-1){s[i]=s[i].substring(s[i].indexOf(">")+1,s[i].length)}}
strx=s.join("")}
chop=(chop<strx.length-1)?chop:strx.length-2;while(strx.charAt(chop-1)!=' '&&strx.indexOf(' ',chop)!=-1)chop++;strx=strx.substring(0,chop-1);return strx+'...'}
function createSummaryAndThumb(pID){var div=document.getElementById(pID);var imgtag="";var img=div.getElementsByTagName("img");var summ=summary_noimg;if(img.length>=1){imgtag='<div class="xopostimg"><img src="'+img[0].src+'" width="100%" alt=""/></div>';summ=summary_img}
var summary=imgtag+'<div class="xopostsummary">'+removeHtmlTag(div.innerHTML,summ)+'</div>';div.innerHTML=summary}
        //]]>
    </script>
    <script type='text/javascript'>
            //<![CDATA[
            /*! jQuery v1.11.1 | (c) 2005, 2014 jQuery Foundation, Inc. | jquery.org/license */
!function(a,b){"object"==typeof module&&"object"==typeof module.exports?module.exports=a.document?b(a,!0):function(a){if(!a.document)throw new Error("jQuery requires a window with a document");return b(a)}:b(a)}("undefined"!=typeof window?window:this,function(a,b){var c=[],d=c.slice,e=c.concat,f=c.push,g=c.indexOf,h={},i=h.toString,j=h.hasOwnProperty,k={},l="1.11.1",m=function(a,b){return new m.fn.init(a,b)},n=/^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g,o=/^-ms-/,p=/-([\da-z])/gi,q=function(a,b){return b.toUpperCase()};m.fn=m.prototype={jquery:l,constructor:m,selector:"",length:0,toArray:function(){return d.call(this)},get:function(a){return null!=a?0>a?this[a+this.length]:this[a]:d.call(this)},pushStack:function(a){var b=m.merge(this.constructor(),a);return b.prevObject=this,b.context=this.context,b},each:function(a,b){return m.each(this,a,b)},map:function(a){return this.pushStack(m.map(this,function(b,c){return a.call(b,c,b)}))},slice:function(){return this.pushStack(d.apply(this,arguments))},first:function(){return this.eq(0)},last:function(){return this.eq(-1)},eq:function(a){var b=this.length,c=+a+(0>a?b:0);return this.pushStack(c>=0&&b>c?[this[c]]:[])},end:function(){return this.prevObject||this.constructor(null)},push:f,sort:c.sort,splice:c.splice},m.extend=m.fn.extend=function(){var a,b,c,d,e,f,g=arguments[0]||{},h=1,i=arguments.length,j=!1;for("boolean"==typeof g&&(j=g,g=arguments[h]||{},h++),"object"==typeof g||m.isFunction(g)||(g={}),h===i&&(g=this,h--);i>h;h++)if(null!=(e=arguments[h]))for(d in e)a=g[d],c=e[d],g!==c&&(j&&c&&(m.isPlainObject(c)||(b=m.isArray(c)))?(b?(b=!1,f=a&&m.isArray(a)?a:[]):f=a&&m.isPlainObject(a)?a:{},g[d]=m.extend(j,f,c)):void 0!==c&&(g[d]=c));return g},m.extend({expando:"jQuery"+(l+Math.random()).replace(/\D/g,""),isReady:!0,error:function(a){throw new Error(a)},noop:function(){},isFunction:function(a){return"function"===m.type(a)},isArray:Array.isArray||function(a){return"array"===m.type(a)},isWindow:function(a){return null!=a&&a==a.window},isNumeric:function(a){return!m.isArray(a)&&a-parseFloat(a)>=0},isEmptyObject:function(a){var b;for(b in a)return!1;return!0},isPlainObject:function(a){var b;if(!a||"object"!==m.type(a)||a.nodeType||m.isWindow(a))return!1;try{if(a.constructor&&!j.call(a,"constructor")&&!j.call(a.constructor.prototype,"isPrototypeOf"))return!1}catch(c){return!1}if(k.ownLast)for(b in a)return j.call(a,b);for(b in a);return void 0===b||j.call(a,b)},type:function(a){return null==a?a+"":"object"==typeof a||"function"==typeof a?h[i.call(a)]||"object":typeof a},globalEval:function(b){b&&m.trim(b)&&(a.execScript||function(b){a.eval.call(a,b)})(b)},camelCase:function(a){return a.replace(o,"ms-").replace(p,q)},nodeName:function(a,b){return a.nodeName&&a.nodeName.toLowerCase()===b.toLowerCase()},each:function(a,b,c){var d,e=0,f=a.length,g=r(a);if(c){if(g){for(;f>e;e++)if(d=b.apply(a[e],c),d===!1)break}else for(e in a)if(d=b.apply(a[e],c),d===!1)break}else if(g){for(;f>e;e++)if(d=b.call(a[e],e,a[e]),d===!1)break}else for(e in a)if(d=b.call(a[e],e,a[e]),d===!1)break;return a},trim:function(a){return null==a?"":(a+"").replace(n,"")},makeArray:function(a,b){var c=b||[];return null!=a&&(r(Object(a))?m.merge(c,"string"==typeof a?[a]:a):f.call(c,a)),c},inArray:function(a,b,c){var d;if(b){if(g)return g.call(b,a,c);for(d=b.length,c=c?0>c?Math.max(0,d+c):c:0;d>c;c++)if(c in b&&b[c]===a)return c}return-1},merge:function(a,b){var c=+b.length,d=0,e=a.length;while(c>d)a[e++]=b[d++];if(c!==c)while(void 0!==b[d])a[e++]=b[d++];return a.length=e,a},grep:function(a,b,c){for(var d,e=[],f=0,g=a.length,h=!c;g>f;f++)d=!b(a[f],f),d!==h&&e.push(a[f]);return e},map:function(a,b,c){var d,f=0,g=a.length,h=r(a),i=[];if(h)for(;g>f;f++)d=b(a[f],f,c),null!=d&&i.push(d);else for(f in a)d=b(a[f],f,c),null!=d&&i.push(d);return e.apply([],i)},guid:1,proxy:function(a,b){var c,e,f;return"string"==typeof b&&(f=a[b],b=a,a=f),m.isFunction(a)?(c=d.call(arguments,2),e=function(){return a.apply(b||this,c.concat(d.call(arguments)))},e.guid=a.guid=a.guid||m.guid++,e):void 0},now:function(){return+new Date},support:k}),m.each("Boolean Number String Function Array Date RegExp Object Error".split(" "),function(a,b){h["[object "+b+"]"]=b.toLowerCase()});function r(a){var b=a.length,c=m.type(a);return"function"===c||m.isWindow(a)?!1:1===a.nodeType&&b?!0:"array"===c||0===b||"number"==typeof b&&b>0&&b-1 in a}var s=function(a){var b,c,d,e,f,g,h,i,j,k,l,m,n,o,p,q,r,s,t,u="sizzle"+-new Date,v=a.document,w=0,x=0,y=gb(),z=gb(),A=gb(),B=function(a,b){return a===b&&(l=!0),0},C="undefined",D=1<<31,E={}.hasOwnProperty,F=[],G=F.pop,H=F.push,I=F.push,J=F.slice,K=F.indexOf||function(a){for(var b=0,c=this.length;c>b;b++)if(this[b]===a)return b;return-1},L="checked|selected|async|autofocus|autoplay|controls|defer|disabled|hidden|ismap|loop|multiple|open|readonly|required|scoped",M="[\\x20\\t\\r\\n\\f]",N="(?:\\\\.|[\\w-]|[^\\x00-\\xa0])+",O=N.replace("w","w#"),P="\\["+M+"*("+N+")(?:"+M+"*([*^$|!~]?=)"+M+"*(?:'((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\"|("+O+"))|)"+M+"*\\]",Q=":("+N+")(?:\\((('((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\")|((?:\\\\.|[^\\\\()[\\]]|"+P+")*)|.*)\\)|)",R=new RegExp("^"+M+"+|((?:^|[^\\\\])(?:\\\\.)*)"+M+"+$","g"),S=new RegExp("^"+M+"*,"+M+"*"),T=new RegExp("^"+M+"*([>+~]|"+M+")"+M+"*"),U=new RegExp("="+M+"*([^\\]'\"]*?)"+M+"*\\]","g"),V=new RegExp(Q),W=new RegExp("^"+O+"$"),X={ID:new RegExp("^#("+N+")"),CLASS:new RegExp("^\\.("+N+")"),TAG:new RegExp("^("+N.replace("w","w*")+")"),ATTR:new RegExp("^"+P),PSEUDO:new RegExp("^"+Q),CHILD:new RegExp("^:(only|first|last|nth|nth-last)-(child|of-type)(?:\\("+M+"*(even|odd|(([+-]|)(\\d*)n|)"+M+"*(?:([+-]|)"+M+"*(\\d+)|))"+M+"*\\)|)","i"),bool:new RegExp("^(?:"+L+")$","i"),needsContext:new RegExp("^"+M+"*[>+~]|:(even|odd|eq|gt|lt|nth|first|last)(?:\\("+M+"*((?:-\\d)?\\d*)"+M+"*\\)|)(?=[^-]|$)","i")},Y=/^(?:input|select|textarea|button)$/i,Z=/^h\d$/i,$=/^[^{]+\{\s*\[native \w/,_=/^(?:#([\w-]+)|(\w+)|\.([\w-]+))$/,ab=/[+~]/,bb=/'|\\/g,cb=new RegExp("\\\\([\\da-f]{1,6}"+M+"?|("+M+")|.)","ig"),db=function(a,b,c){var d="0x"+b-65536;return d!==d||c?b:0>d?String.fromCharCode(d+65536):String.fromCharCode(d>>10|55296,1023&d|56320)};try{I.apply(F=J.call(v.childNodes),v.childNodes),F[v.childNodes.length].nodeType}catch(eb){I={apply:F.length?function(a,b){H.apply(a,J.call(b))}:function(a,b){var c=a.length,d=0;while(a[c++]=b[d++]);a.length=c-1}}}function fb(a,b,d,e){var f,h,j,k,l,o,r,s,w,x;if((b?b.ownerDocument||b:v)!==n&&m(b),b=b||n,d=d||[],!a||"string"!=typeof a)return d;if(1!==(k=b.nodeType)&&9!==k)return[];if(p&&!e){if(f=_.exec(a))if(j=f[1]){if(9===k){if(h=b.getElementById(j),!h||!h.parentNode)return d;if(h.id===j)return d.push(h),d}else if(b.ownerDocument&&(h=b.ownerDocument.getElementById(j))&&t(b,h)&&h.id===j)return d.push(h),d}else{if(f[2])return I.apply(d,b.getElementsByTagName(a)),d;if((j=f[3])&&c.getElementsByClassName&&b.getElementsByClassName)return I.apply(d,b.getElementsByClassName(j)),d}if(c.qsa&&(!q||!q.test(a))){if(s=r=u,w=b,x=9===k&&a,1===k&&"object"!==b.nodeName.toLowerCase()){o=g(a),(r=b.getAttribute("id"))?s=r.replace(bb,"\\$&"):b.setAttribute("id",s),s="[id='"+s+"'] ",l=o.length;while(l--)o[l]=s+qb(o[l]);w=ab.test(a)&&ob(b.parentNode)||b,x=o.join(",")}if(x)try{return I.apply(d,w.querySelectorAll(x)),d}catch(y){}finally{r||b.removeAttribute("id")}}}return i(a.replace(R,"$1"),b,d,e)}function gb(){var a=[];function b(c,e){return a.push(c+" ")>d.cacheLength&&delete b[a.shift()],b[c+" "]=e}return b}function hb(a){return a[u]=!0,a}function ib(a){var b=n.createElement("div");try{return!!a(b)}catch(c){return!1}finally{b.parentNode&&b.parentNode.removeChild(b),b=null}}function jb(a,b){var c=a.split("|"),e=a.length;while(e--)d.attrHandle[c[e]]=b}function kb(a,b){var c=b&&a,d=c&&1===a.nodeType&&1===b.nodeType&&(~b.sourceIndex||D)-(~a.sourceIndex||D);if(d)return d;if(c)while(c=c.nextSibling)if(c===b)return-1;return a?1:-1}function lb(a){return function(b){var c=b.nodeName.toLowerCase();return"input"===c&&b.type===a}}function mb(a){return function(b){var c=b.nodeName.toLowerCase();return("input"===c||"button"===c)&&b.type===a}}function nb(a){return hb(function(b){return b=+b,hb(function(c,d){var e,f=a([],c.length,b),g=f.length;while(g--)c[e=f[g]]&&(c[e]=!(d[e]=c[e]))})})}function ob(a){return a&&typeof a.getElementsByTagName!==C&&a}c=fb.support={},f=fb.isXML=function(a){var b=a&&(a.ownerDocument||a).documentElement;return b?"HTML"!==b.nodeName:!1},m=fb.setDocument=function(a){var b,e=a?a.ownerDocument||a:v,g=e.defaultView;return e!==n&&9===e.nodeType&&e.documentElement?(n=e,o=e.documentElement,p=!f(e),g&&g!==g.top&&(g.addEventListener?g.addEventListener("unload",function(){m()},!1):g.attachEvent&&g.attachEvent("onunload",function(){m()})),c.attributes=ib(function(a){return a.className="i",!a.getAttribute("className")}),c.getElementsByTagName=ib(function(a){return a.appendChild(e.createComment("")),!a.getElementsByTagName("*").length}),c.getElementsByClassName=$.test(e.getElementsByClassName)&&ib(function(a){return a.innerHTML="<div class='a'></div><div class='a i'></div>",a.firstChild.className="i",2===a.getElementsByClassName("i").length}),c.getById=ib(function(a){return o.appendChild(a).id=u,!e.getElementsByName||!e.getElementsByName(u).length}),c.getById?(d.find.ID=function(a,b){if(typeof b.getElementById!==C&&p){var c=b.getElementById(a);return c&&c.parentNode?[c]:[]}},d.filter.ID=function(a){var b=a.replace(cb,db);return function(a){return a.getAttribute("id")===b}}):(delete d.find.ID,d.filter.ID=function(a){var b=a.replace(cb,db);return function(a){var c=typeof a.getAttributeNode!==C&&a.getAttributeNode("id");return c&&c.value===b}}),d.find.TAG=c.getElementsByTagName?function(a,b){return typeof b.getElementsByTagName!==C?b.getElementsByTagName(a):void 0}:function(a,b){var c,d=[],e=0,f=b.getElementsByTagName(a);if("*"===a){while(c=f[e++])1===c.nodeType&&d.push(c);return d}return f},d.find.CLASS=c.getElementsByClassName&&function(a,b){return typeof b.getElementsByClassName!==C&&p?b.getElementsByClassName(a):void 0},r=[],q=[],(c.qsa=$.test(e.querySelectorAll))&&(ib(function(a){a.innerHTML="<select msallowclip=''><option selected=''></option></select>",a.querySelectorAll("[msallowclip^='']").length&&q.push("[*^$]="+M+"*(?:''|\"\")"),a.querySelectorAll("[selected]").length||q.push("\\["+M+"*(?:value|"+L+")"),a.querySelectorAll(":checked").length||q.push(":checked")}),ib(function(a){var b=e.createElement("input");b.setAttribute("type","hidden"),a.appendChild(b).setAttribute("name","D"),a.querySelectorAll("[name=d]").length&&q.push("name"+M+"*[*^$|!~]?="),a.querySelectorAll(":enabled").length||q.push(":enabled",":disabled"),a.querySelectorAll("*,:x"),q.push(",.*:")})),(c.matchesSelector=$.test(s=o.matches||o.webkitMatchesSelector||o.mozMatchesSelector||o.oMatchesSelector||o.msMatchesSelector))&&ib(function(a){c.disconnectedMatch=s.call(a,"div"),s.call(a,"[s!='']:x"),r.push("!=",Q)}),q=q.length&&new RegExp(q.join("|")),r=r.length&&new RegExp(r.join("|")),b=$.test(o.compareDocumentPosition),t=b||$.test(o.contains)?function(a,b){var c=9===a.nodeType?a.documentElement:a,d=b&&b.parentNode;return a===d||!(!d||1!==d.nodeType||!(c.contains?c.contains(d):a.compareDocumentPosition&&16&a.compareDocumentPosition(d)))}:function(a,b){if(b)while(b=b.parentNode)if(b===a)return!0;return!1},B=b?function(a,b){if(a===b)return l=!0,0;var d=!a.compareDocumentPosition-!b.compareDocumentPosition;return d?d:(d=(a.ownerDocument||a)===(b.ownerDocument||b)?a.compareDocumentPosition(b):1,1&d||!c.sortDetached&&b.compareDocumentPosition(a)===d?a===e||a.ownerDocument===v&&t(v,a)?-1:b===e||b.ownerDocument===v&&t(v,b)?1:k?K.call(k,a)-K.call(k,b):0:4&d?-1:1)}:function(a,b){if(a===b)return l=!0,0;var c,d=0,f=a.parentNode,g=b.parentNode,h=[a],i=[b];if(!f||!g)return a===e?-1:b===e?1:f?-1:g?1:k?K.call(k,a)-K.call(k,b):0;if(f===g)return kb(a,b);c=a;while(c=c.parentNode)h.unshift(c);c=b;while(c=c.parentNode)i.unshift(c);while(h[d]===i[d])d++;return d?kb(h[d],i[d]):h[d]===v?-1:i[d]===v?1:0},e):n},fb.matches=function(a,b){return fb(a,null,null,b)},fb.matchesSelector=function(a,b){if((a.ownerDocument||a)!==n&&m(a),b=b.replace(U,"='$1']"),!(!c.matchesSelector||!p||r&&r.test(b)||q&&q.test(b)))try{var d=s.call(a,b);if(d||c.disconnectedMatch||a.document&&11!==a.document.nodeType)return d}catch(e){}return fb(b,n,null,[a]).length>0},fb.contains=function(a,b){return(a.ownerDocument||a)!==n&&m(a),t(a,b)},fb.attr=function(a,b){(a.ownerDocument||a)!==n&&m(a);var e=d.attrHandle[b.toLowerCase()],f=e&&E.call(d.attrHandle,b.toLowerCase())?e(a,b,!p):void 0;return void 0!==f?f:c.attributes||!p?a.getAttribute(b):(f=a.getAttributeNode(b))&&f.specified?f.value:null},fb.error=function(a){throw new Error("Syntax error, unrecognized expression: "+a)},fb.uniqueSort=function(a){var b,d=[],e=0,f=0;if(l=!c.detectDuplicates,k=!c.sortStable&&a.slice(0),a.sort(B),l){while(b=a[f++])b===a[f]&&(e=d.push(f));while(e--)a.splice(d[e],1)}return k=null,a},e=fb.getText=function(a){var b,c="",d=0,f=a.nodeType;if(f){if(1===f||9===f||11===f){if("string"==typeof a.textContent)return a.textContent;for(a=a.firstChild;a;a=a.nextSibling)c+=e(a)}else if(3===f||4===f)return a.nodeValue}else while(b=a[d++])c+=e(b);return c},d=fb.selectors={cacheLength:50,createPseudo:hb,match:X,attrHandle:{},find:{},relative:{">":{dir:"parentNode",first:!0}," ":{dir:"parentNode"},"+":{dir:"previousSibling",first:!0},"~":{dir:"previousSibling"}},preFilter:{ATTR:function(a){return a[1]=a[1].replace(cb,db),a[3]=(a[3]||a[4]||a[5]||"").replace(cb,db),"~="===a[2]&&(a[3]=" "+a[3]+" "),a.slice(0,4)},CHILD:function(a){return a[1]=a[1].toLowerCase(),"nth"===a[1].slice(0,3)?(a[3]||fb.error(a[0]),a[4]=+(a[4]?a[5]+(a[6]||1):2*("even"===a[3]||"odd"===a[3])),a[5]=+(a[7]+a[8]||"odd"===a[3])):a[3]&&fb.error(a[0]),a},PSEUDO:function(a){var b,c=!a[6]&&a[2];return X.CHILD.test(a[0])?null:(a[3]?a[2]=a[4]||a[5]||"":c&&V.test(c)&&(b=g(c,!0))&&(b=c.indexOf(")",c.length-b)-c.length)&&(a[0]=a[0].slice(0,b),a[2]=c.slice(0,b)),a.slice(0,3))}},filter:{TAG:function(a){var b=a.replace(cb,db).toLowerCase();return"*"===a?function(){return!0}:function(a){return a.nodeName&&a.nodeName.toLowerCase()===b}},CLASS:function(a){var b=y[a+" "];return b||(b=new RegExp("(^|"+M+")"+a+"("+M+"|$)"))&&y(a,function(a){return b.test("string"==typeof a.className&&a.className||typeof a.getAttribute!==C&&a.getAttribute("class")||"")})},ATTR:function(a,b,c){return function(d){var e=fb.attr(d,a);return null==e?"!="===b:b?(e+="","="===b?e===c:"!="===b?e!==c:"^="===b?c&&0===e.indexOf(c):"*="===b?c&&e.indexOf(c)>-1:"$="===b?c&&e.slice(-c.length)===c:"~="===b?(" "+e+" ").indexOf(c)>-1:"|="===b?e===c||e.slice(0,c.length+1)===c+"-":!1):!0}},CHILD:function(a,b,c,d,e){var f="nth"!==a.slice(0,3),g="last"!==a.slice(-4),h="of-type"===b;return 1===d&&0===e?function(a){return!!a.parentNode}:function(b,c,i){var j,k,l,m,n,o,p=f!==g?"nextSibling":"previousSibling",q=b.parentNode,r=h&&b.nodeName.toLowerCase(),s=!i&&!h;if(q){if(f){while(p){l=b;while(l=l[p])if(h?l.nodeName.toLowerCase()===r:1===l.nodeType)return!1;o=p="only"===a&&!o&&"nextSibling"}return!0}if(o=[g?q.firstChild:q.lastChild],g&&s){k=q[u]||(q[u]={}),j=k[a]||[],n=j[0]===w&&j[1],m=j[0]===w&&j[2],l=n&&q.childNodes[n];while(l=++n&&l&&l[p]||(m=n=0)||o.pop())if(1===l.nodeType&&++m&&l===b){k[a]=[w,n,m];break}}else if(s&&(j=(b[u]||(b[u]={}))[a])&&j[0]===w)m=j[1];else while(l=++n&&l&&l[p]||(m=n=0)||o.pop())if((h?l.nodeName.toLowerCase()===r:1===l.nodeType)&&++m&&(s&&((l[u]||(l[u]={}))[a]=[w,m]),l===b))break;return m-=e,m===d||m%d===0&&m/d>=0}}},PSEUDO:function(a,b){var c,e=d.pseudos[a]||d.setFilters[a.toLowerCase()]||fb.error("unsupported pseudo: "+a);return e[u]?e(b):e.length>1?(c=[a,a,"",b],d.setFilters.hasOwnProperty(a.toLowerCase())?hb(function(a,c){var d,f=e(a,b),g=f.length;while(g--)d=K.call(a,f[g]),a[d]=!(c[d]=f[g])}):function(a){return e(a,0,c)}):e}},pseudos:{not:hb(function(a){var b=[],c=[],d=h(a.replace(R,"$1"));return d[u]?hb(function(a,b,c,e){var f,g=d(a,null,e,[]),h=a.length;while(h--)(f=g[h])&&(a[h]=!(b[h]=f))}):function(a,e,f){return b[0]=a,d(b,null,f,c),!c.pop()}}),has:hb(function(a){return function(b){return fb(a,b).length>0}}),contains:hb(function(a){return function(b){return(b.textContent||b.innerText||e(b)).indexOf(a)>-1}}),lang:hb(function(a){return W.test(a||"")||fb.error("unsupported lang: "+a),a=a.replace(cb,db).toLowerCase(),function(b){var c;do if(c=p?b.lang:b.getAttribute("xml:lang")||b.getAttribute("lang"))return c=c.toLowerCase(),c===a||0===c.indexOf(a+"-");while((b=b.parentNode)&&1===b.nodeType);return!1}}),target:function(b){var c=a.location&&a.location.hash;return c&&c.slice(1)===b.id},root:function(a){return a===o},focus:function(a){return a===n.activeElement&&(!n.hasFocus||n.hasFocus())&&!!(a.type||a.href||~a.tabIndex)},enabled:function(a){return a.disabled===!1},disabled:function(a){return a.disabled===!0},checked:function(a){var b=a.nodeName.toLowerCase();return"input"===b&&!!a.checked||"option"===b&&!!a.selected},selected:function(a){return a.parentNode&&a.parentNode.selectedIndex,a.selected===!0},empty:function(a){for(a=a.firstChild;a;a=a.nextSibling)if(a.nodeType<6)return!1;return!0},parent:function(a){return!d.pseudos.empty(a)},header:function(a){return Z.test(a.nodeName)},input:function(a){return Y.test(a.nodeName)},button:function(a){var b=a.nodeName.toLowerCase();return"input"===b&&"button"===a.type||"button"===b},text:function(a){var b;return"input"===a.nodeName.toLowerCase()&&"text"===a.type&&(null==(b=a.getAttribute("type"))||"text"===b.toLowerCase())},first:nb(function(){return[0]}),last:nb(function(a,b){return[b-1]}),eq:nb(function(a,b,c){return[0>c?c+b:c]}),even:nb(function(a,b){for(var c=0;b>c;c+=2)a.push(c);return a}),odd:nb(function(a,b){for(var c=1;b>c;c+=2)a.push(c);return a}),lt:nb(function(a,b,c){for(var d=0>c?c+b:c;--d>=0;)a.push(d);return a}),gt:nb(function(a,b,c){for(var d=0>c?c+b:c;++d<b;)a.push(d);return a})}},d.pseudos.nth=d.pseudos.eq;for(b in{radio:!0,checkbox:!0,file:!0,password:!0,image:!0})d.pseudos[b]=lb(b);for(b in{submit:!0,reset:!0})d.pseudos[b]=mb(b);function pb(){}pb.prototype=d.filters=d.pseudos,d.setFilters=new pb,g=fb.tokenize=function(a,b){var c,e,f,g,h,i,j,k=z[a+" "];if(k)return b?0:k.slice(0);h=a,i=[],j=d.preFilter;while(h){(!c||(e=S.exec(h)))&&(e&&(h=h.slice(e[0].length)||h),i.push(f=[])),c=!1,(e=T.exec(h))&&(c=e.shift(),f.push({value:c,type:e[0].replace(R," ")}),h=h.slice(c.length));for(g in d.filter)!(e=X[g].exec(h))||j[g]&&!(e=j[g](e))||(c=e.shift(),f.push({value:c,type:g,matches:e}),h=h.slice(c.length));if(!c)break}return b?h.length:h?fb.error(a):z(a,i).slice(0)};function qb(a){for(var b=0,c=a.length,d="";c>b;b++)d+=a[b].value;return d}function rb(a,b,c){var d=b.dir,e=c&&"parentNode"===d,f=x++;return b.first?function(b,c,f){while(b=b[d])if(1===b.nodeType||e)return a(b,c,f)}:function(b,c,g){var h,i,j=[w,f];if(g){while(b=b[d])if((1===b.nodeType||e)&&a(b,c,g))return!0}else while(b=b[d])if(1===b.nodeType||e){if(i=b[u]||(b[u]={}),(h=i[d])&&h[0]===w&&h[1]===f)return j[2]=h[2];if(i[d]=j,j[2]=a(b,c,g))return!0}}}function sb(a){return a.length>1?function(b,c,d){var e=a.length;while(e--)if(!a[e](b,c,d))return!1;return!0}:a[0]}function tb(a,b,c){for(var d=0,e=b.length;e>d;d++)fb(a,b[d],c);return c}function ub(a,b,c,d,e){for(var f,g=[],h=0,i=a.length,j=null!=b;i>h;h++)(f=a[h])&&(!c||c(f,d,e))&&(g.push(f),j&&b.push(h));return g}function vb(a,b,c,d,e,f){return d&&!d[u]&&(d=vb(d)),e&&!e[u]&&(e=vb(e,f)),hb(function(f,g,h,i){var j,k,l,m=[],n=[],o=g.length,p=f||tb(b||"*",h.nodeType?[h]:h,[]),q=!a||!f&&b?p:ub(p,m,a,h,i),r=c?e||(f?a:o||d)?[]:g:q;if(c&&c(q,r,h,i),d){j=ub(r,n),d(j,[],h,i),k=j.length;while(k--)(l=j[k])&&(r[n[k]]=!(q[n[k]]=l))}if(f){if(e||a){if(e){j=[],k=r.length;while(k--)(l=r[k])&&j.push(q[k]=l);e(null,r=[],j,i)}k=r.length;while(k--)(l=r[k])&&(j=e?K.call(f,l):m[k])>-1&&(f[j]=!(g[j]=l))}}else r=ub(r===g?r.splice(o,r.length):r),e?e(null,g,r,i):I.apply(g,r)})}function wb(a){for(var b,c,e,f=a.length,g=d.relative[a[0].type],h=g||d.relative[" "],i=g?1:0,k=rb(function(a){return a===b},h,!0),l=rb(function(a){return K.call(b,a)>-1},h,!0),m=[function(a,c,d){return!g&&(d||c!==j)||((b=c).nodeType?k(a,c,d):l(a,c,d))}];f>i;i++)if(c=d.relative[a[i].type])m=[rb(sb(m),c)];else{if(c=d.filter[a[i].type].apply(null,a[i].matches),c[u]){for(e=++i;f>e;e++)if(d.relative[a[e].type])break;return vb(i>1&&sb(m),i>1&&qb(a.slice(0,i-1).concat({value:" "===a[i-2].type?"*":""})).replace(R,"$1"),c,e>i&&wb(a.slice(i,e)),f>e&&wb(a=a.slice(e)),f>e&&qb(a))}m.push(c)}return sb(m)}function xb(a,b){var c=b.length>0,e=a.length>0,f=function(f,g,h,i,k){var l,m,o,p=0,q="0",r=f&&[],s=[],t=j,u=f||e&&d.find.TAG("*",k),v=w+=null==t?1:Math.random()||.1,x=u.length;for(k&&(j=g!==n&&g);q!==x&&null!=(l=u[q]);q++){if(e&&l){m=0;while(o=a[m++])if(o(l,g,h)){i.push(l);break}k&&(w=v)}c&&((l=!o&&l)&&p--,f&&r.push(l))}if(p+=q,c&&q!==p){m=0;while(o=b[m++])o(r,s,g,h);if(f){if(p>0)while(q--)r[q]||s[q]||(s[q]=G.call(i));s=ub(s)}I.apply(i,s),k&&!f&&s.length>0&&p+b.length>1&&fb.uniqueSort(i)}return k&&(w=v,j=t),r};return c?hb(f):f}return h=fb.compile=function(a,b){var c,d=[],e=[],f=A[a+" "];if(!f){b||(b=g(a)),c=b.length;while(c--)f=wb(b[c]),f[u]?d.push(f):e.push(f);f=A(a,xb(e,d)),f.selector=a}return f},i=fb.select=function(a,b,e,f){var i,j,k,l,m,n="function"==typeof a&&a,o=!f&&g(a=n.selector||a);if(e=e||[],1===o.length){if(j=o[0]=o[0].slice(0),j.length>2&&"ID"===(k=j[0]).type&&c.getById&&9===b.nodeType&&p&&d.relative[j[1].type]){if(b=(d.find.ID(k.matches[0].replace(cb,db),b)||[])[0],!b)return e;n&&(b=b.parentNode),a=a.slice(j.shift().value.length)}i=X.needsContext.test(a)?0:j.length;while(i--){if(k=j[i],d.relative[l=k.type])break;if((m=d.find[l])&&(f=m(k.matches[0].replace(cb,db),ab.test(j[0].type)&&ob(b.parentNode)||b))){if(j.splice(i,1),a=f.length&&qb(j),!a)return I.apply(e,f),e;break}}}return(n||h(a,o))(f,b,!p,e,ab.test(a)&&ob(b.parentNode)||b),e},c.sortStable=u.split("").sort(B).join("")===u,c.detectDuplicates=!!l,m(),c.sortDetached=ib(function(a){return 1&a.compareDocumentPosition(n.createElement("div"))}),ib(function(a){return a.innerHTML="<a href='#'></a>","#"===a.firstChild.getAttribute("href")})||jb("type|href|height|width",function(a,b,c){return c?void 0:a.getAttribute(b,"type"===b.toLowerCase()?1:2)}),c.attributes&&ib(function(a){return a.innerHTML="<input/>",a.firstChild.setAttribute("value",""),""===a.firstChild.getAttribute("value")})||jb("value",function(a,b,c){return c||"input"!==a.nodeName.toLowerCase()?void 0:a.defaultValue}),ib(function(a){return null==a.getAttribute("disabled")})||jb(L,function(a,b,c){var d;return c?void 0:a[b]===!0?b.toLowerCase():(d=a.getAttributeNode(b))&&d.specified?d.value:null}),fb}(a);m.find=s,m.expr=s.selectors,m.expr[":"]=m.expr.pseudos,m.unique=s.uniqueSort,m.text=s.getText,m.isXMLDoc=s.isXML,m.contains=s.contains;var t=m.expr.match.needsContext,u=/^<(\w+)\s*\/?>(?:<\/\1>|)$/,v=/^.[^:#\[\.,]*$/;function w(a,b,c){if(m.isFunction(b))return m.grep(a,function(a,d){return!!b.call(a,d,a)!==c});if(b.nodeType)return m.grep(a,function(a){return a===b!==c});if("string"==typeof b){if(v.test(b))return m.filter(b,a,c);b=m.filter(b,a)}return m.grep(a,function(a){return m.inArray(a,b)>=0!==c})}m.filter=function(a,b,c){var d=b[0];return c&&(a=":not("+a+")"),1===b.length&&1===d.nodeType?m.find.matchesSelector(d,a)?[d]:[]:m.find.matches(a,m.grep(b,function(a){return 1===a.nodeType}))},m.fn.extend({find:function(a){var b,c=[],d=this,e=d.length;if("string"!=typeof a)return this.pushStack(m(a).filter(function(){for(b=0;e>b;b++)if(m.contains(d[b],this))return!0}));for(b=0;e>b;b++)m.find(a,d[b],c);return c=this.pushStack(e>1?m.unique(c):c),c.selector=this.selector?this.selector+" "+a:a,c},filter:function(a){return this.pushStack(w(this,a||[],!1))},not:function(a){return this.pushStack(w(this,a||[],!0))},is:function(a){return!!w(this,"string"==typeof a&&t.test(a)?m(a):a||[],!1).length}});var x,y=a.document,z=/^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]*))$/,A=m.fn.init=function(a,b){var c,d;if(!a)return this;if("string"==typeof a){if(c="<"===a.charAt(0)&&">"===a.charAt(a.length-1)&&a.length>=3?[null,a,null]:z.exec(a),!c||!c[1]&&b)return!b||b.jquery?(b||x).find(a):this.constructor(b).find(a);if(c[1]){if(b=b instanceof m?b[0]:b,m.merge(this,m.parseHTML(c[1],b&&b.nodeType?b.ownerDocument||b:y,!0)),u.test(c[1])&&m.isPlainObject(b))for(c in b)m.isFunction(this[c])?this[c](b[c]):this.attr(c,b[c]);return this}if(d=y.getElementById(c[2]),d&&d.parentNode){if(d.id!==c[2])return x.find(a);this.length=1,this[0]=d}return this.context=y,this.selector=a,this}return a.nodeType?(this.context=this[0]=a,this.length=1,this):m.isFunction(a)?"undefined"!=typeof x.ready?x.ready(a):a(m):(void 0!==a.selector&&(this.selector=a.selector,this.context=a.context),m.makeArray(a,this))};A.prototype=m.fn,x=m(y);var B=/^(?:parents|prev(?:Until|All))/,C={children:!0,contents:!0,next:!0,prev:!0};m.extend({dir:function(a,b,c){var d=[],e=a[b];while(e&&9!==e.nodeType&&(void 0===c||1!==e.nodeType||!m(e).is(c)))1===e.nodeType&&d.push(e),e=e[b];return d},sibling:function(a,b){for(var c=[];a;a=a.nextSibling)1===a.nodeType&&a!==b&&c.push(a);return c}}),m.fn.extend({has:function(a){var b,c=m(a,this),d=c.length;return this.filter(function(){for(b=0;d>b;b++)if(m.contains(this,c[b]))return!0})},closest:function(a,b){for(var c,d=0,e=this.length,f=[],g=t.test(a)||"string"!=typeof a?m(a,b||this.context):0;e>d;d++)for(c=this[d];c&&c!==b;c=c.parentNode)if(c.nodeType<11&&(g?g.index(c)>-1:1===c.nodeType&&m.find.matchesSelector(c,a))){f.push(c);break}return this.pushStack(f.length>1?m.unique(f):f)},index:function(a){return a?"string"==typeof a?m.inArray(this[0],m(a)):m.inArray(a.jquery?a[0]:a,this):this[0]&&this[0].parentNode?this.first().prevAll().length:-1},add:function(a,b){return this.pushStack(m.unique(m.merge(this.get(),m(a,b))))},addBack:function(a){return this.add(null==a?this.prevObject:this.prevObject.filter(a))}});function D(a,b){do a=a[b];while(a&&1!==a.nodeType);return a}m.each({parent:function(a){var b=a.parentNode;return b&&11!==b.nodeType?b:null},parents:function(a){return m.dir(a,"parentNode")},parentsUntil:function(a,b,c){return m.dir(a,"parentNode",c)},next:function(a){return D(a,"nextSibling")},prev:function(a){return D(a,"previousSibling")},nextAll:function(a){return m.dir(a,"nextSibling")},prevAll:function(a){return m.dir(a,"previousSibling")},nextUntil:function(a,b,c){return m.dir(a,"nextSibling",c)},prevUntil:function(a,b,c){return m.dir(a,"previousSibling",c)},siblings:function(a){return m.sibling((a.parentNode||{}).firstChild,a)},children:function(a){return m.sibling(a.firstChild)},contents:function(a){return m.nodeName(a,"iframe")?a.contentDocument||a.contentWindow.document:m.merge([],a.childNodes)}},function(a,b){m.fn[a]=function(c,d){var e=m.map(this,b,c);return"Until"!==a.slice(-5)&&(d=c),d&&"string"==typeof d&&(e=m.filter(d,e)),this.length>1&&(C[a]||(e=m.unique(e)),B.test(a)&&(e=e.reverse())),this.pushStack(e)}});var E=/\S+/g,F={};function G(a){var b=F[a]={};return m.each(a.match(E)||[],function(a,c){b[c]=!0}),b}m.Callbacks=function(a){a="string"==typeof a?F[a]||G(a):m.extend({},a);var b,c,d,e,f,g,h=[],i=!a.once&&[],j=function(l){for(c=a.memory&&l,d=!0,f=g||0,g=0,e=h.length,b=!0;h&&e>f;f++)if(h[f].apply(l[0],l[1])===!1&&a.stopOnFalse){c=!1;break}b=!1,h&&(i?i.length&&j(i.shift()):c?h=[]:k.disable())},k={add:function(){if(h){var d=h.length;!function f(b){m.each(b,function(b,c){var d=m.type(c);"function"===d?a.unique&&k.has(c)||h.push(c):c&&c.length&&"string"!==d&&f(c)})}(arguments),b?e=h.length:c&&(g=d,j(c))}return this},remove:function(){return h&&m.each(arguments,function(a,c){var d;while((d=m.inArray(c,h,d))>-1)h.splice(d,1),b&&(e>=d&&e--,f>=d&&f--)}),this},has:function(a){return a?m.inArray(a,h)>-1:!(!h||!h.length)},empty:function(){return h=[],e=0,this},disable:function(){return h=i=c=void 0,this},disabled:function(){return!h},lock:function(){return i=void 0,c||k.disable(),this},locked:function(){return!i},fireWith:function(a,c){return!h||d&&!i||(c=c||[],c=[a,c.slice?c.slice():c],b?i.push(c):j(c)),this},fire:function(){return k.fireWith(this,arguments),this},fired:function(){return!!d}};return k},m.extend({Deferred:function(a){var b=[["resolve","done",m.Callbacks("once memory"),"resolved"],["reject","fail",m.Callbacks("once memory"),"rejected"],["notify","progress",m.Callbacks("memory")]],c="pending",d={state:function(){return c},always:function(){return e.done(arguments).fail(arguments),this},then:function(){var a=arguments;return m.Deferred(function(c){m.each(b,function(b,f){var g=m.isFunction(a[b])&&a[b];e[f[1]](function(){var a=g&&g.apply(this,arguments);a&&m.isFunction(a.promise)?a.promise().done(c.resolve).fail(c.reject).progress(c.notify):c[f[0]+"With"](this===d?c.promise():this,g?[a]:arguments)})}),a=null}).promise()},promise:function(a){return null!=a?m.extend(a,d):d}},e={};return d.pipe=d.then,m.each(b,function(a,f){var g=f[2],h=f[3];d[f[1]]=g.add,h&&g.add(function(){c=h},b[1^a][2].disable,b[2][2].lock),e[f[0]]=function(){return e[f[0]+"With"](this===e?d:this,arguments),this},e[f[0]+"With"]=g.fireWith}),d.promise(e),a&&a.call(e,e),e},when:function(a){var b=0,c=d.call(arguments),e=c.length,f=1!==e||a&&m.isFunction(a.promise)?e:0,g=1===f?a:m.Deferred(),h=function(a,b,c){return function(e){b[a]=this,c[a]=arguments.length>1?d.call(arguments):e,c===i?g.notifyWith(b,c):--f||g.resolveWith(b,c)}},i,j,k;if(e>1)for(i=new Array(e),j=new Array(e),k=new Array(e);e>b;b++)c[b]&&m.isFunction(c[b].promise)?c[b].promise().done(h(b,k,c)).fail(g.reject).progress(h(b,j,i)):--f;return f||g.resolveWith(k,c),g.promise()}});var H;m.fn.ready=function(a){return m.ready.promise().done(a),this},m.extend({isReady:!1,readyWait:1,holdReady:function(a){a?m.readyWait++:m.ready(!0)},ready:function(a){if(a===!0?!--m.readyWait:!m.isReady){if(!y.body)return setTimeout(m.ready);m.isReady=!0,a!==!0&&--m.readyWait>0||(H.resolveWith(y,[m]),m.fn.triggerHandler&&(m(y).triggerHandler("ready"),m(y).off("ready")))}}});function I(){y.addEventListener?(y.removeEventListener("DOMContentLoaded",J,!1),a.removeEventListener("load",J,!1)):(y.detachEvent("onreadystatechange",J),a.detachEvent("onload",J))}function J(){(y.addEventListener||"load"===event.type||"complete"===y.readyState)&&(I(),m.ready())}m.ready.promise=function(b){if(!H)if(H=m.Deferred(),"complete"===y.readyState)setTimeout(m.ready);else if(y.addEventListener)y.addEventListener("DOMContentLoaded",J,!1),a.addEventListener("load",J,!1);else{y.attachEvent("onreadystatechange",J),a.attachEvent("onload",J);var c=!1;try{c=null==a.frameElement&&y.documentElement}catch(d){}c&&c.doScroll&&!function e(){if(!m.isReady){try{c.doScroll("left")}catch(a){return setTimeout(e,50)}I(),m.ready()}}()}return H.promise(b)};var K="undefined",L;for(L in m(k))break;k.ownLast="0"!==L,k.inlineBlockNeedsLayout=!1,m(function(){var a,b,c,d;c=y.getElementsByTagName("body")[0],c&&c.style&&(b=y.createElement("div"),d=y.createElement("div"),d.style.cssText="position:absolute;border:0;width:0;height:0;top:0;left:-9999px",c.appendChild(d).appendChild(b),typeof b.style.zoom!==K&&(b.style.cssText="display:inline;margin:0;border:0;padding:1px;width:1px;zoom:1",k.inlineBlockNeedsLayout=a=3===b.offsetWidth,a&&(c.style.zoom=1)),c.removeChild(d))}),function(){var a=y.createElement("div");if(null==k.deleteExpando){k.deleteExpando=!0;try{delete a.test}catch(b){k.deleteExpando=!1}}a=null}(),m.acceptData=function(a){var b=m.noData[(a.nodeName+" ").toLowerCase()],c=+a.nodeType||1;return 1!==c&&9!==c?!1:!b||b!==!0&&a.getAttribute("classid")===b};var M=/^(?:\{[\w\W]*\}|\[[\w\W]*\])$/,N=/([A-Z])/g;function O(a,b,c){if(void 0===c&&1===a.nodeType){var d="data-"+b.replace(N,"-$1").toLowerCase();if(c=a.getAttribute(d),"string"==typeof c){try{c="true"===c?!0:"false"===c?!1:"null"===c?null:+c+""===c?+c:M.test(c)?m.parseJSON(c):c}catch(e){}m.data(a,b,c)}else c=void 0}return c}function P(a){var b;for(b in a)if(("data"!==b||!m.isEmptyObject(a[b]))&&"toJSON"!==b)return!1;return!0}function Q(a,b,d,e){if(m.acceptData(a)){var f,g,h=m.expando,i=a.nodeType,j=i?m.cache:a,k=i?a[h]:a[h]&&h;
if(k&&j[k]&&(e||j[k].data)||void 0!==d||"string"!=typeof b)return k||(k=i?a[h]=c.pop()||m.guid++:h),j[k]||(j[k]=i?{}:{toJSON:m.noop}),("object"==typeof b||"function"==typeof b)&&(e?j[k]=m.extend(j[k],b):j[k].data=m.extend(j[k].data,b)),g=j[k],e||(g.data||(g.data={}),g=g.data),void 0!==d&&(g[m.camelCase(b)]=d),"string"==typeof b?(f=g[b],null==f&&(f=g[m.camelCase(b)])):f=g,f}}function R(a,b,c){if(m.acceptData(a)){var d,e,f=a.nodeType,g=f?m.cache:a,h=f?a[m.expando]:m.expando;if(g[h]){if(b&&(d=c?g[h]:g[h].data)){m.isArray(b)?b=b.concat(m.map(b,m.camelCase)):b in d?b=[b]:(b=m.camelCase(b),b=b in d?[b]:b.split(" ")),e=b.length;while(e--)delete d[b[e]];if(c?!P(d):!m.isEmptyObject(d))return}(c||(delete g[h].data,P(g[h])))&&(f?m.cleanData([a],!0):k.deleteExpando||g!=g.window?delete g[h]:g[h]=null)}}}m.extend({cache:{},noData:{"applet ":!0,"embed ":!0,"object ":"clsid:D27CDB6E-AE6D-11cf-96B8-444553540000"},hasData:function(a){return a=a.nodeType?m.cache[a[m.expando]]:a[m.expando],!!a&&!P(a)},data:function(a,b,c){return Q(a,b,c)},removeData:function(a,b){return R(a,b)},_data:function(a,b,c){return Q(a,b,c,!0)},_removeData:function(a,b){return R(a,b,!0)}}),m.fn.extend({data:function(a,b){var c,d,e,f=this[0],g=f&&f.attributes;if(void 0===a){if(this.length&&(e=m.data(f),1===f.nodeType&&!m._data(f,"parsedAttrs"))){c=g.length;while(c--)g[c]&&(d=g[c].name,0===d.indexOf("data-")&&(d=m.camelCase(d.slice(5)),O(f,d,e[d])));m._data(f,"parsedAttrs",!0)}return e}return"object"==typeof a?this.each(function(){m.data(this,a)}):arguments.length>1?this.each(function(){m.data(this,a,b)}):f?O(f,a,m.data(f,a)):void 0},removeData:function(a){return this.each(function(){m.removeData(this,a)})}}),m.extend({queue:function(a,b,c){var d;return a?(b=(b||"fx")+"queue",d=m._data(a,b),c&&(!d||m.isArray(c)?d=m._data(a,b,m.makeArray(c)):d.push(c)),d||[]):void 0},dequeue:function(a,b){b=b||"fx";var c=m.queue(a,b),d=c.length,e=c.shift(),f=m._queueHooks(a,b),g=function(){m.dequeue(a,b)};"inprogress"===e&&(e=c.shift(),d--),e&&("fx"===b&&c.unshift("inprogress"),delete f.stop,e.call(a,g,f)),!d&&f&&f.empty.fire()},_queueHooks:function(a,b){var c=b+"queueHooks";return m._data(a,c)||m._data(a,c,{empty:m.Callbacks("once memory").add(function(){m._removeData(a,b+"queue"),m._removeData(a,c)})})}}),m.fn.extend({queue:function(a,b){var c=2;return"string"!=typeof a&&(b=a,a="fx",c--),arguments.length<c?m.queue(this[0],a):void 0===b?this:this.each(function(){var c=m.queue(this,a,b);m._queueHooks(this,a),"fx"===a&&"inprogress"!==c[0]&&m.dequeue(this,a)})},dequeue:function(a){return this.each(function(){m.dequeue(this,a)})},clearQueue:function(a){return this.queue(a||"fx",[])},promise:function(a,b){var c,d=1,e=m.Deferred(),f=this,g=this.length,h=function(){--d||e.resolveWith(f,[f])};"string"!=typeof a&&(b=a,a=void 0),a=a||"fx";while(g--)c=m._data(f[g],a+"queueHooks"),c&&c.empty&&(d++,c.empty.add(h));return h(),e.promise(b)}});var S=/[+-]?(?:\d*\.|)\d+(?:[eE][+-]?\d+|)/.source,T=["Top","Right","Bottom","Left"],U=function(a,b){return a=b||a,"none"===m.css(a,"display")||!m.contains(a.ownerDocument,a)},V=m.access=function(a,b,c,d,e,f,g){var h=0,i=a.length,j=null==c;if("object"===m.type(c)){e=!0;for(h in c)m.access(a,b,h,c[h],!0,f,g)}else if(void 0!==d&&(e=!0,m.isFunction(d)||(g=!0),j&&(g?(b.call(a,d),b=null):(j=b,b=function(a,b,c){return j.call(m(a),c)})),b))for(;i>h;h++)b(a[h],c,g?d:d.call(a[h],h,b(a[h],c)));return e?a:j?b.call(a):i?b(a[0],c):f},W=/^(?:checkbox|radio)$/i;!function(){var a=y.createElement("input"),b=y.createElement("div"),c=y.createDocumentFragment();if(b.innerHTML="  <link/><table></table><a href='/a'>a</a><input type='checkbox'/>",k.leadingWhitespace=3===b.firstChild.nodeType,k.tbody=!b.getElementsByTagName("tbody").length,k.htmlSerialize=!!b.getElementsByTagName("link").length,k.html5Clone="<:nav></:nav>"!==y.createElement("nav").cloneNode(!0).outerHTML,a.type="checkbox",a.checked=!0,c.appendChild(a),k.appendChecked=a.checked,b.innerHTML="<textarea>x</textarea>",k.noCloneChecked=!!b.cloneNode(!0).lastChild.defaultValue,c.appendChild(b),b.innerHTML="<input type='radio' checked='checked' name='t'/>",k.checkClone=b.cloneNode(!0).cloneNode(!0).lastChild.checked,k.noCloneEvent=!0,b.attachEvent&&(b.attachEvent("onclick",function(){k.noCloneEvent=!1}),b.cloneNode(!0).click()),null==k.deleteExpando){k.deleteExpando=!0;try{delete b.test}catch(d){k.deleteExpando=!1}}}(),function(){var b,c,d=y.createElement("div");for(b in{submit:!0,change:!0,focusin:!0})c="on"+b,(k[b+"Bubbles"]=c in a)||(d.setAttribute(c,"t"),k[b+"Bubbles"]=d.attributes[c].expando===!1);d=null}();var X=/^(?:input|select|textarea)$/i,Y=/^key/,Z=/^(?:mouse|pointer|contextmenu)|click/,$=/^(?:focusinfocus|focusoutblur)$/,_=/^([^.]*)(?:\.(.+)|)$/;function ab(){return!0}function bb(){return!1}function cb(){try{return y.activeElement}catch(a){}}m.event={global:{},add:function(a,b,c,d,e){var f,g,h,i,j,k,l,n,o,p,q,r=m._data(a);if(r){c.handler&&(i=c,c=i.handler,e=i.selector),c.guid||(c.guid=m.guid++),(g=r.events)||(g=r.events={}),(k=r.handle)||(k=r.handle=function(a){return typeof m===K||a&&m.event.triggered===a.type?void 0:m.event.dispatch.apply(k.elem,arguments)},k.elem=a),b=(b||"").match(E)||[""],h=b.length;while(h--)f=_.exec(b[h])||[],o=q=f[1],p=(f[2]||"").split(".").sort(),o&&(j=m.event.special[o]||{},o=(e?j.delegateType:j.bindType)||o,j=m.event.special[o]||{},l=m.extend({type:o,origType:q,data:d,handler:c,guid:c.guid,selector:e,needsContext:e&&m.expr.match.needsContext.test(e),namespace:p.join(".")},i),(n=g[o])||(n=g[o]=[],n.delegateCount=0,j.setup&&j.setup.call(a,d,p,k)!==!1||(a.addEventListener?a.addEventListener(o,k,!1):a.attachEvent&&a.attachEvent("on"+o,k))),j.add&&(j.add.call(a,l),l.handler.guid||(l.handler.guid=c.guid)),e?n.splice(n.delegateCount++,0,l):n.push(l),m.event.global[o]=!0);a=null}},remove:function(a,b,c,d,e){var f,g,h,i,j,k,l,n,o,p,q,r=m.hasData(a)&&m._data(a);if(r&&(k=r.events)){b=(b||"").match(E)||[""],j=b.length;while(j--)if(h=_.exec(b[j])||[],o=q=h[1],p=(h[2]||"").split(".").sort(),o){l=m.event.special[o]||{},o=(d?l.delegateType:l.bindType)||o,n=k[o]||[],h=h[2]&&new RegExp("(^|\\.)"+p.join("\\.(?:.*\\.|)")+"(\\.|$)"),i=f=n.length;while(f--)g=n[f],!e&&q!==g.origType||c&&c.guid!==g.guid||h&&!h.test(g.namespace)||d&&d!==g.selector&&("**"!==d||!g.selector)||(n.splice(f,1),g.selector&&n.delegateCount--,l.remove&&l.remove.call(a,g));i&&!n.length&&(l.teardown&&l.teardown.call(a,p,r.handle)!==!1||m.removeEvent(a,o,r.handle),delete k[o])}else for(o in k)m.event.remove(a,o+b[j],c,d,!0);m.isEmptyObject(k)&&(delete r.handle,m._removeData(a,"events"))}},trigger:function(b,c,d,e){var f,g,h,i,k,l,n,o=[d||y],p=j.call(b,"type")?b.type:b,q=j.call(b,"namespace")?b.namespace.split("."):[];if(h=l=d=d||y,3!==d.nodeType&&8!==d.nodeType&&!$.test(p+m.event.triggered)&&(p.indexOf(".")>=0&&(q=p.split("."),p=q.shift(),q.sort()),g=p.indexOf(":")<0&&"on"+p,b=b[m.expando]?b:new m.Event(p,"object"==typeof b&&b),b.isTrigger=e?2:3,b.namespace=q.join("."),b.namespace_re=b.namespace?new RegExp("(^|\\.)"+q.join("\\.(?:.*\\.|)")+"(\\.|$)"):null,b.result=void 0,b.target||(b.target=d),c=null==c?[b]:m.makeArray(c,[b]),k=m.event.special[p]||{},e||!k.trigger||k.trigger.apply(d,c)!==!1)){if(!e&&!k.noBubble&&!m.isWindow(d)){for(i=k.delegateType||p,$.test(i+p)||(h=h.parentNode);h;h=h.parentNode)o.push(h),l=h;l===(d.ownerDocument||y)&&o.push(l.defaultView||l.parentWindow||a)}n=0;while((h=o[n++])&&!b.isPropagationStopped())b.type=n>1?i:k.bindType||p,f=(m._data(h,"events")||{})[b.type]&&m._data(h,"handle"),f&&f.apply(h,c),f=g&&h[g],f&&f.apply&&m.acceptData(h)&&(b.result=f.apply(h,c),b.result===!1&&b.preventDefault());if(b.type=p,!e&&!b.isDefaultPrevented()&&(!k._default||k._default.apply(o.pop(),c)===!1)&&m.acceptData(d)&&g&&d[p]&&!m.isWindow(d)){l=d[g],l&&(d[g]=null),m.event.triggered=p;try{d[p]()}catch(r){}m.event.triggered=void 0,l&&(d[g]=l)}return b.result}},dispatch:function(a){a=m.event.fix(a);var b,c,e,f,g,h=[],i=d.call(arguments),j=(m._data(this,"events")||{})[a.type]||[],k=m.event.special[a.type]||{};if(i[0]=a,a.delegateTarget=this,!k.preDispatch||k.preDispatch.call(this,a)!==!1){h=m.event.handlers.call(this,a,j),b=0;while((f=h[b++])&&!a.isPropagationStopped()){a.currentTarget=f.elem,g=0;while((e=f.handlers[g++])&&!a.isImmediatePropagationStopped())(!a.namespace_re||a.namespace_re.test(e.namespace))&&(a.handleObj=e,a.data=e.data,c=((m.event.special[e.origType]||{}).handle||e.handler).apply(f.elem,i),void 0!==c&&(a.result=c)===!1&&(a.preventDefault(),a.stopPropagation()))}return k.postDispatch&&k.postDispatch.call(this,a),a.result}},handlers:function(a,b){var c,d,e,f,g=[],h=b.delegateCount,i=a.target;if(h&&i.nodeType&&(!a.button||"click"!==a.type))for(;i!=this;i=i.parentNode||this)if(1===i.nodeType&&(i.disabled!==!0||"click"!==a.type)){for(e=[],f=0;h>f;f++)d=b[f],c=d.selector+" ",void 0===e[c]&&(e[c]=d.needsContext?m(c,this).index(i)>=0:m.find(c,this,null,[i]).length),e[c]&&e.push(d);e.length&&g.push({elem:i,handlers:e})}return h<b.length&&g.push({elem:this,handlers:b.slice(h)}),g},fix:function(a){if(a[m.expando])return a;var b,c,d,e=a.type,f=a,g=this.fixHooks[e];g||(this.fixHooks[e]=g=Z.test(e)?this.mouseHooks:Y.test(e)?this.keyHooks:{}),d=g.props?this.props.concat(g.props):this.props,a=new m.Event(f),b=d.length;while(b--)c=d[b],a[c]=f[c];return a.target||(a.target=f.srcElement||y),3===a.target.nodeType&&(a.target=a.target.parentNode),a.metaKey=!!a.metaKey,g.filter?g.filter(a,f):a},props:"altKey bubbles cancelable ctrlKey currentTarget eventPhase metaKey relatedTarget shiftKey target timeStamp view which".split(" "),fixHooks:{},keyHooks:{props:"char charCode key keyCode".split(" "),filter:function(a,b){return null==a.which&&(a.which=null!=b.charCode?b.charCode:b.keyCode),a}},mouseHooks:{props:"button buttons clientX clientY fromElement offsetX offsetY pageX pageY screenX screenY toElement".split(" "),filter:function(a,b){var c,d,e,f=b.button,g=b.fromElement;return null==a.pageX&&null!=b.clientX&&(d=a.target.ownerDocument||y,e=d.documentElement,c=d.body,a.pageX=b.clientX+(e&&e.scrollLeft||c&&c.scrollLeft||0)-(e&&e.clientLeft||c&&c.clientLeft||0),a.pageY=b.clientY+(e&&e.scrollTop||c&&c.scrollTop||0)-(e&&e.clientTop||c&&c.clientTop||0)),!a.relatedTarget&&g&&(a.relatedTarget=g===a.target?b.toElement:g),a.which||void 0===f||(a.which=1&f?1:2&f?3:4&f?2:0),a}},special:{load:{noBubble:!0},focus:{trigger:function(){if(this!==cb()&&this.focus)try{return this.focus(),!1}catch(a){}},delegateType:"focusin"},blur:{trigger:function(){return this===cb()&&this.blur?(this.blur(),!1):void 0},delegateType:"focusout"},click:{trigger:function(){return m.nodeName(this,"input")&&"checkbox"===this.type&&this.click?(this.click(),!1):void 0},_default:function(a){return m.nodeName(a.target,"a")}},beforeunload:{postDispatch:function(a){void 0!==a.result&&a.originalEvent&&(a.originalEvent.returnValue=a.result)}}},simulate:function(a,b,c,d){var e=m.extend(new m.Event,c,{type:a,isSimulated:!0,originalEvent:{}});d?m.event.trigger(e,null,b):m.event.dispatch.call(b,e),e.isDefaultPrevented()&&c.preventDefault()}},m.removeEvent=y.removeEventListener?function(a,b,c){a.removeEventListener&&a.removeEventListener(b,c,!1)}:function(a,b,c){var d="on"+b;a.detachEvent&&(typeof a[d]===K&&(a[d]=null),a.detachEvent(d,c))},m.Event=function(a,b){return this instanceof m.Event?(a&&a.type?(this.originalEvent=a,this.type=a.type,this.isDefaultPrevented=a.defaultPrevented||void 0===a.defaultPrevented&&a.returnValue===!1?ab:bb):this.type=a,b&&m.extend(this,b),this.timeStamp=a&&a.timeStamp||m.now(),void(this[m.expando]=!0)):new m.Event(a,b)},m.Event.prototype={isDefaultPrevented:bb,isPropagationStopped:bb,isImmediatePropagationStopped:bb,preventDefault:function(){var a=this.originalEvent;this.isDefaultPrevented=ab,a&&(a.preventDefault?a.preventDefault():a.returnValue=!1)},stopPropagation:function(){var a=this.originalEvent;this.isPropagationStopped=ab,a&&(a.stopPropagation&&a.stopPropagation(),a.cancelBubble=!0)},stopImmediatePropagation:function(){var a=this.originalEvent;this.isImmediatePropagationStopped=ab,a&&a.stopImmediatePropagation&&a.stopImmediatePropagation(),this.stopPropagation()}},m.each({mouseenter:"mouseover",mouseleave:"mouseout",pointerenter:"pointerover",pointerleave:"pointerout"},function(a,b){m.event.special[a]={delegateType:b,bindType:b,handle:function(a){var c,d=this,e=a.relatedTarget,f=a.handleObj;return(!e||e!==d&&!m.contains(d,e))&&(a.type=f.origType,c=f.handler.apply(this,arguments),a.type=b),c}}}),k.submitBubbles||(m.event.special.submit={setup:function(){return m.nodeName(this,"form")?!1:void m.event.add(this,"click._submit keypress._submit",function(a){var b=a.target,c=m.nodeName(b,"input")||m.nodeName(b,"button")?b.form:void 0;c&&!m._data(c,"submitBubbles")&&(m.event.add(c,"submit._submit",function(a){a._submit_bubble=!0}),m._data(c,"submitBubbles",!0))})},postDispatch:function(a){a._submit_bubble&&(delete a._submit_bubble,this.parentNode&&!a.isTrigger&&m.event.simulate("submit",this.parentNode,a,!0))},teardown:function(){return m.nodeName(this,"form")?!1:void m.event.remove(this,"._submit")}}),k.changeBubbles||(m.event.special.change={setup:function(){return X.test(this.nodeName)?(("checkbox"===this.type||"radio"===this.type)&&(m.event.add(this,"propertychange._change",function(a){"checked"===a.originalEvent.propertyName&&(this._just_changed=!0)}),m.event.add(this,"click._change",function(a){this._just_changed&&!a.isTrigger&&(this._just_changed=!1),m.event.simulate("change",this,a,!0)})),!1):void m.event.add(this,"beforeactivate._change",function(a){var b=a.target;X.test(b.nodeName)&&!m._data(b,"changeBubbles")&&(m.event.add(b,"change._change",function(a){!this.parentNode||a.isSimulated||a.isTrigger||m.event.simulate("change",this.parentNode,a,!0)}),m._data(b,"changeBubbles",!0))})},handle:function(a){var b=a.target;return this!==b||a.isSimulated||a.isTrigger||"radio"!==b.type&&"checkbox"!==b.type?a.handleObj.handler.apply(this,arguments):void 0},teardown:function(){return m.event.remove(this,"._change"),!X.test(this.nodeName)}}),k.focusinBubbles||m.each({focus:"focusin",blur:"focusout"},function(a,b){var c=function(a){m.event.simulate(b,a.target,m.event.fix(a),!0)};m.event.special[b]={setup:function(){var d=this.ownerDocument||this,e=m._data(d,b);e||d.addEventListener(a,c,!0),m._data(d,b,(e||0)+1)},teardown:function(){var d=this.ownerDocument||this,e=m._data(d,b)-1;e?m._data(d,b,e):(d.removeEventListener(a,c,!0),m._removeData(d,b))}}}),m.fn.extend({on:function(a,b,c,d,e){var f,g;if("object"==typeof a){"string"!=typeof b&&(c=c||b,b=void 0);for(f in a)this.on(f,b,c,a[f],e);return this}if(null==c&&null==d?(d=b,c=b=void 0):null==d&&("string"==typeof b?(d=c,c=void 0):(d=c,c=b,b=void 0)),d===!1)d=bb;else if(!d)return this;return 1===e&&(g=d,d=function(a){return m().off(a),g.apply(this,arguments)},d.guid=g.guid||(g.guid=m.guid++)),this.each(function(){m.event.add(this,a,d,c,b)})},one:function(a,b,c,d){return this.on(a,b,c,d,1)},off:function(a,b,c){var d,e;if(a&&a.preventDefault&&a.handleObj)return d=a.handleObj,m(a.delegateTarget).off(d.namespace?d.origType+"."+d.namespace:d.origType,d.selector,d.handler),this;if("object"==typeof a){for(e in a)this.off(e,b,a[e]);return this}return(b===!1||"function"==typeof b)&&(c=b,b=void 0),c===!1&&(c=bb),this.each(function(){m.event.remove(this,a,c,b)})},trigger:function(a,b){return this.each(function(){m.event.trigger(a,b,this)})},triggerHandler:function(a,b){var c=this[0];return c?m.event.trigger(a,b,c,!0):void 0}});function db(a){var b=eb.split("|"),c=a.createDocumentFragment();if(c.createElement)while(b.length)c.createElement(b.pop());return c}var eb="abbr|article|aside|audio|bdi|canvas|data|datalist|details|figcaption|figure|footer|header|hgroup|mark|meter|nav|output|progress|section|summary|time|video",fb=/ jQuery\d+="(?:null|\d+)"/g,gb=new RegExp("<(?:"+eb+")[\\s/>]","i"),hb=/^\s+/,ib=/<(?!area|br|col|embed|hr|img|input|link|meta|param)(([\w:]+)[^>]*)\/>/gi,jb=/<([\w:]+)/,kb=/<tbody/i,lb=/<|&#?\w+;/,mb=/<(?:script|style|link)/i,nb=/checked\s*(?:[^=]|=\s*.checked.)/i,ob=/^$|\/(?:java|ecma)script/i,pb=/^true\/(.*)/,qb=/^\s*<!(?:\[CDATA\[|--)|(?:\]\]|--)>\s*$/g,rb={option:[1,"<select multiple='multiple'>","</select>"],legend:[1,"<fieldset>","</fieldset>"],area:[1,"<map>","</map>"],param:[1,"<object>","</object>"],thead:[1,"<table>","</table>"],tr:[2,"<table><tbody>","</tbody></table>"],col:[2,"<table><tbody></tbody><colgroup>","</colgroup></table>"],td:[3,"<table><tbody><tr>","</tr></tbody></table>"],_default:k.htmlSerialize?[0,"",""]:[1,"X<div>","</div>"]},sb=db(y),tb=sb.appendChild(y.createElement("div"));rb.optgroup=rb.option,rb.tbody=rb.tfoot=rb.colgroup=rb.caption=rb.thead,rb.th=rb.td;function ub(a,b){var c,d,e=0,f=typeof a.getElementsByTagName!==K?a.getElementsByTagName(b||"*"):typeof a.querySelectorAll!==K?a.querySelectorAll(b||"*"):void 0;if(!f)for(f=[],c=a.childNodes||a;null!=(d=c[e]);e++)!b||m.nodeName(d,b)?f.push(d):m.merge(f,ub(d,b));return void 0===b||b&&m.nodeName(a,b)?m.merge([a],f):f}function vb(a){W.test(a.type)&&(a.defaultChecked=a.checked)}function wb(a,b){return m.nodeName(a,"table")&&m.nodeName(11!==b.nodeType?b:b.firstChild,"tr")?a.getElementsByTagName("tbody")[0]||a.appendChild(a.ownerDocument.createElement("tbody")):a}function xb(a){return a.type=(null!==m.find.attr(a,"type"))+"/"+a.type,a}function yb(a){var b=pb.exec(a.type);return b?a.type=b[1]:a.removeAttribute("type"),a}function zb(a,b){for(var c,d=0;null!=(c=a[d]);d++)m._data(c,"globalEval",!b||m._data(b[d],"globalEval"))}function Ab(a,b){if(1===b.nodeType&&m.hasData(a)){var c,d,e,f=m._data(a),g=m._data(b,f),h=f.events;if(h){delete g.handle,g.events={};for(c in h)for(d=0,e=h[c].length;e>d;d++)m.event.add(b,c,h[c][d])}g.data&&(g.data=m.extend({},g.data))}}function Bb(a,b){var c,d,e;if(1===b.nodeType){if(c=b.nodeName.toLowerCase(),!k.noCloneEvent&&b[m.expando]){e=m._data(b);for(d in e.events)m.removeEvent(b,d,e.handle);b.removeAttribute(m.expando)}"script"===c&&b.text!==a.text?(xb(b).text=a.text,yb(b)):"object"===c?(b.parentNode&&(b.outerHTML=a.outerHTML),k.html5Clone&&a.innerHTML&&!m.trim(b.innerHTML)&&(b.innerHTML=a.innerHTML)):"input"===c&&W.test(a.type)?(b.defaultChecked=b.checked=a.checked,b.value!==a.value&&(b.value=a.value)):"option"===c?b.defaultSelected=b.selected=a.defaultSelected:("input"===c||"textarea"===c)&&(b.defaultValue=a.defaultValue)}}m.extend({clone:function(a,b,c){var d,e,f,g,h,i=m.contains(a.ownerDocument,a);if(k.html5Clone||m.isXMLDoc(a)||!gb.test("<"+a.nodeName+">")?f=a.cloneNode(!0):(tb.innerHTML=a.outerHTML,tb.removeChild(f=tb.firstChild)),!(k.noCloneEvent&&k.noCloneChecked||1!==a.nodeType&&11!==a.nodeType||m.isXMLDoc(a)))for(d=ub(f),h=ub(a),g=0;null!=(e=h[g]);++g)d[g]&&Bb(e,d[g]);if(b)if(c)for(h=h||ub(a),d=d||ub(f),g=0;null!=(e=h[g]);g++)Ab(e,d[g]);else Ab(a,f);return d=ub(f,"script"),d.length>0&&zb(d,!i&&ub(a,"script")),d=h=e=null,f},buildFragment:function(a,b,c,d){for(var e,f,g,h,i,j,l,n=a.length,o=db(b),p=[],q=0;n>q;q++)if(f=a[q],f||0===f)if("object"===m.type(f))m.merge(p,f.nodeType?[f]:f);else if(lb.test(f)){h=h||o.appendChild(b.createElement("div")),i=(jb.exec(f)||["",""])[1].toLowerCase(),l=rb[i]||rb._default,h.innerHTML=l[1]+f.replace(ib,"<$1></$2>")+l[2],e=l[0];while(e--)h=h.lastChild;if(!k.leadingWhitespace&&hb.test(f)&&p.push(b.createTextNode(hb.exec(f)[0])),!k.tbody){f="table"!==i||kb.test(f)?"<table>"!==l[1]||kb.test(f)?0:h:h.firstChild,e=f&&f.childNodes.length;while(e--)m.nodeName(j=f.childNodes[e],"tbody")&&!j.childNodes.length&&f.removeChild(j)}m.merge(p,h.childNodes),h.textContent="";while(h.firstChild)h.removeChild(h.firstChild);h=o.lastChild}else p.push(b.createTextNode(f));h&&o.removeChild(h),k.appendChecked||m.grep(ub(p,"input"),vb),q=0;while(f=p[q++])if((!d||-1===m.inArray(f,d))&&(g=m.contains(f.ownerDocument,f),h=ub(o.appendChild(f),"script"),g&&zb(h),c)){e=0;while(f=h[e++])ob.test(f.type||"")&&c.push(f)}return h=null,o},cleanData:function(a,b){for(var d,e,f,g,h=0,i=m.expando,j=m.cache,l=k.deleteExpando,n=m.event.special;null!=(d=a[h]);h++)if((b||m.acceptData(d))&&(f=d[i],g=f&&j[f])){if(g.events)for(e in g.events)n[e]?m.event.remove(d,e):m.removeEvent(d,e,g.handle);j[f]&&(delete j[f],l?delete d[i]:typeof d.removeAttribute!==K?d.removeAttribute(i):d[i]=null,c.push(f))}}}),m.fn.extend({text:function(a){return V(this,function(a){return void 0===a?m.text(this):this.empty().append((this[0]&&this[0].ownerDocument||y).createTextNode(a))},null,a,arguments.length)},append:function(){return this.domManip(arguments,function(a){if(1===this.nodeType||11===this.nodeType||9===this.nodeType){var b=wb(this,a);b.appendChild(a)}})},prepend:function(){return this.domManip(arguments,function(a){if(1===this.nodeType||11===this.nodeType||9===this.nodeType){var b=wb(this,a);b.insertBefore(a,b.firstChild)}})},before:function(){return this.domManip(arguments,function(a){this.parentNode&&this.parentNode.insertBefore(a,this)})},after:function(){return this.domManip(arguments,function(a){this.parentNode&&this.parentNode.insertBefore(a,this.nextSibling)})},remove:function(a,b){for(var c,d=a?m.filter(a,this):this,e=0;null!=(c=d[e]);e++)b||1!==c.nodeType||m.cleanData(ub(c)),c.parentNode&&(b&&m.contains(c.ownerDocument,c)&&zb(ub(c,"script")),c.parentNode.removeChild(c));return this},empty:function(){for(var a,b=0;null!=(a=this[b]);b++){1===a.nodeType&&m.cleanData(ub(a,!1));while(a.firstChild)a.removeChild(a.firstChild);a.options&&m.nodeName(a,"select")&&(a.options.length=0)}return this},clone:function(a,b){return a=null==a?!1:a,b=null==b?a:b,this.map(function(){return m.clone(this,a,b)})},html:function(a){return V(this,function(a){var b=this[0]||{},c=0,d=this.length;if(void 0===a)return 1===b.nodeType?b.innerHTML.replace(fb,""):void 0;if(!("string"!=typeof a||mb.test(a)||!k.htmlSerialize&&gb.test(a)||!k.leadingWhitespace&&hb.test(a)||rb[(jb.exec(a)||["",""])[1].toLowerCase()])){a=a.replace(ib,"<$1></$2>");try{for(;d>c;c++)b=this[c]||{},1===b.nodeType&&(m.cleanData(ub(b,!1)),b.innerHTML=a);b=0}catch(e){}}b&&this.empty().append(a)},null,a,arguments.length)},replaceWith:function(){var a=arguments[0];return this.domManip(arguments,function(b){a=this.parentNode,m.cleanData(ub(this)),a&&a.replaceChild(b,this)}),a&&(a.length||a.nodeType)?this:this.remove()},detach:function(a){return this.remove(a,!0)},domManip:function(a,b){a=e.apply([],a);var c,d,f,g,h,i,j=0,l=this.length,n=this,o=l-1,p=a[0],q=m.isFunction(p);if(q||l>1&&"string"==typeof p&&!k.checkClone&&nb.test(p))return this.each(function(c){var d=n.eq(c);q&&(a[0]=p.call(this,c,d.html())),d.domManip(a,b)});if(l&&(i=m.buildFragment(a,this[0].ownerDocument,!1,this),c=i.firstChild,1===i.childNodes.length&&(i=c),c)){for(g=m.map(ub(i,"script"),xb),f=g.length;l>j;j++)d=i,j!==o&&(d=m.clone(d,!0,!0),f&&m.merge(g,ub(d,"script"))),b.call(this[j],d,j);if(f)for(h=g[g.length-1].ownerDocument,m.map(g,yb),j=0;f>j;j++)d=g[j],ob.test(d.type||"")&&!m._data(d,"globalEval")&&m.contains(h,d)&&(d.src?m._evalUrl&&m._evalUrl(d.src):m.globalEval((d.text||d.textContent||d.innerHTML||"").replace(qb,"")));i=c=null}return this}}),m.each({appendTo:"append",prependTo:"prepend",insertBefore:"before",insertAfter:"after",replaceAll:"replaceWith"},function(a,b){m.fn[a]=function(a){for(var c,d=0,e=[],g=m(a),h=g.length-1;h>=d;d++)c=d===h?this:this.clone(!0),m(g[d])[b](c),f.apply(e,c.get());return this.pushStack(e)}});var Cb,Db={};function Eb(b,c){var d,e=m(c.createElement(b)).appendTo(c.body),f=a.getDefaultComputedStyle&&(d=a.getDefaultComputedStyle(e[0]))?d.display:m.css(e[0],"display");return e.detach(),f}function Fb(a){var b=y,c=Db[a];return c||(c=Eb(a,b),"none"!==c&&c||(Cb=(Cb||m("<iframe frameborder='0' width='0' height='0'/>")).appendTo(b.documentElement),b=(Cb[0].contentWindow||Cb[0].contentDocument).document,b.write(),b.close(),c=Eb(a,b),Cb.detach()),Db[a]=c),c}!function(){var a;k.shrinkWrapBlocks=function(){if(null!=a)return a;a=!1;var b,c,d;return c=y.getElementsByTagName("body")[0],c&&c.style?(b=y.createElement("div"),d=y.createElement("div"),d.style.cssText="position:absolute;border:0;width:0;height:0;top:0;left:-9999px",c.appendChild(d).appendChild(b),typeof b.style.zoom!==K&&(b.style.cssText="-webkit-box-sizing:content-box;-moz-box-sizing:content-box;box-sizing:content-box;display:block;margin:0;border:0;padding:1px;width:1px;zoom:1",b.appendChild(y.createElement("div")).style.width="5px",a=3!==b.offsetWidth),c.removeChild(d),a):void 0}}();var Gb=/^margin/,Hb=new RegExp("^("+S+")(?!px)[a-z%]+$","i"),Ib,Jb,Kb=/^(top|right|bottom|left)$/;a.getComputedStyle?(Ib=function(a){return a.ownerDocument.defaultView.getComputedStyle(a,null)},Jb=function(a,b,c){var d,e,f,g,h=a.style;return c=c||Ib(a),g=c?c.getPropertyValue(b)||c[b]:void 0,c&&(""!==g||m.contains(a.ownerDocument,a)||(g=m.style(a,b)),Hb.test(g)&&Gb.test(b)&&(d=h.width,e=h.minWidth,f=h.maxWidth,h.minWidth=h.maxWidth=h.width=g,g=c.width,h.width=d,h.minWidth=e,h.maxWidth=f)),void 0===g?g:g+""}):y.documentElement.currentStyle&&(Ib=function(a){return a.currentStyle},Jb=function(a,b,c){var d,e,f,g,h=a.style;return c=c||Ib(a),g=c?c[b]:void 0,null==g&&h&&h[b]&&(g=h[b]),Hb.test(g)&&!Kb.test(b)&&(d=h.left,e=a.runtimeStyle,f=e&&e.left,f&&(e.left=a.currentStyle.left),h.left="fontSize"===b?"1em":g,g=h.pixelLeft+"px",h.left=d,f&&(e.left=f)),void 0===g?g:g+""||"auto"});function Lb(a,b){return{get:function(){var c=a();if(null!=c)return c?void delete this.get:(this.get=b).apply(this,arguments)}}}!function(){var b,c,d,e,f,g,h;if(b=y.createElement("div"),b.innerHTML="  <link/><table></table><a href='/a'>a</a><input type='checkbox'/>",d=b.getElementsByTagName("a")[0],c=d&&d.style){c.cssText="float:left;opacity:.5",k.opacity="0.5"===c.opacity,k.cssFloat=!!c.cssFloat,b.style.backgroundClip="content-box",b.cloneNode(!0).style.backgroundClip="",k.clearCloneStyle="content-box"===b.style.backgroundClip,k.boxSizing=""===c.boxSizing||""===c.MozBoxSizing||""===c.WebkitBoxSizing,m.extend(k,{reliableHiddenOffsets:function(){return null==g&&i(),g},boxSizingReliable:function(){return null==f&&i(),f},pixelPosition:function(){return null==e&&i(),e},reliableMarginRight:function(){return null==h&&i(),h}});function i(){var b,c,d,i;c=y.getElementsByTagName("body")[0],c&&c.style&&(b=y.createElement("div"),d=y.createElement("div"),d.style.cssText="position:absolute;border:0;width:0;height:0;top:0;left:-9999px",c.appendChild(d).appendChild(b),b.style.cssText="-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box;display:block;margin-top:1%;top:1%;border:1px;padding:1px;width:4px;position:absolute",e=f=!1,h=!0,a.getComputedStyle&&(e="1%"!==(a.getComputedStyle(b,null)||{}).top,f="4px"===(a.getComputedStyle(b,null)||{width:"4px"}).width,i=b.appendChild(y.createElement("div")),i.style.cssText=b.style.cssText="-webkit-box-sizing:content-box;-moz-box-sizing:content-box;box-sizing:content-box;display:block;margin:0;border:0;padding:0",i.style.marginRight=i.style.width="0",b.style.width="1px",h=!parseFloat((a.getComputedStyle(i,null)||{}).marginRight)),b.innerHTML="<table><tr><td></td><td>t</td></tr></table>",i=b.getElementsByTagName("td"),i[0].style.cssText="margin:0;border:0;padding:0;display:none",g=0===i[0].offsetHeight,g&&(i[0].style.display="",i[1].style.display="none",g=0===i[0].offsetHeight),c.removeChild(d))}}}(),m.swap=function(a,b,c,d){var e,f,g={};for(f in b)g[f]=a.style[f],a.style[f]=b[f];e=c.apply(a,d||[]);for(f in b)a.style[f]=g[f];return e};var Mb=/alpha\([^)]*\)/i,Nb=/opacity\s*=\s*([^)]*)/,Ob=/^(none|table(?!-c[ea]).+)/,Pb=new RegExp("^("+S+")(.*)$","i"),Qb=new RegExp("^([+-])=("+S+")","i"),Rb={position:"absolute",visibility:"hidden",display:"block"},Sb={letterSpacing:"0",fontWeight:"400"},Tb=["Webkit","O","Moz","ms"];function Ub(a,b){if(b in a)return b;var c=b.charAt(0).toUpperCase()+b.slice(1),d=b,e=Tb.length;while(e--)if(b=Tb[e]+c,b in a)return b;return d}function Vb(a,b){for(var c,d,e,f=[],g=0,h=a.length;h>g;g++)d=a[g],d.style&&(f[g]=m._data(d,"olddisplay"),c=d.style.display,b?(f[g]||"none"!==c||(d.style.display=""),""===d.style.display&&U(d)&&(f[g]=m._data(d,"olddisplay",Fb(d.nodeName)))):(e=U(d),(c&&"none"!==c||!e)&&m._data(d,"olddisplay",e?c:m.css(d,"display"))));for(g=0;h>g;g++)d=a[g],d.style&&(b&&"none"!==d.style.display&&""!==d.style.display||(d.style.display=b?f[g]||"":"none"));return a}function Wb(a,b,c){var d=Pb.exec(b);return d?Math.max(0,d[1]-(c||0))+(d[2]||"px"):b}function Xb(a,b,c,d,e){for(var f=c===(d?"border":"content")?4:"width"===b?1:0,g=0;4>f;f+=2)"margin"===c&&(g+=m.css(a,c+T[f],!0,e)),d?("content"===c&&(g-=m.css(a,"padding"+T[f],!0,e)),"margin"!==c&&(g-=m.css(a,"border"+T[f]+"Width",!0,e))):(g+=m.css(a,"padding"+T[f],!0,e),"padding"!==c&&(g+=m.css(a,"border"+T[f]+"Width",!0,e)));return g}function Yb(a,b,c){var d=!0,e="width"===b?a.offsetWidth:a.offsetHeight,f=Ib(a),g=k.boxSizing&&"border-box"===m.css(a,"boxSizing",!1,f);if(0>=e||null==e){if(e=Jb(a,b,f),(0>e||null==e)&&(e=a.style[b]),Hb.test(e))return e;d=g&&(k.boxSizingReliable()||e===a.style[b]),e=parseFloat(e)||0}return e+Xb(a,b,c||(g?"border":"content"),d,f)+"px"}m.extend({cssHooks:{opacity:{get:function(a,b){if(b){var c=Jb(a,"opacity");return""===c?"1":c}}}},cssNumber:{columnCount:!0,fillOpacity:!0,flexGrow:!0,flexShrink:!0,fontWeight:!0,lineHeight:!0,opacity:!0,order:!0,orphans:!0,widows:!0,zIndex:!0,zoom:!0},cssProps:{"float":k.cssFloat?"cssFloat":"styleFloat"},style:function(a,b,c,d){if(a&&3!==a.nodeType&&8!==a.nodeType&&a.style){var e,f,g,h=m.camelCase(b),i=a.style;if(b=m.cssProps[h]||(m.cssProps[h]=Ub(i,h)),g=m.cssHooks[b]||m.cssHooks[h],void 0===c)return g&&"get"in g&&void 0!==(e=g.get(a,!1,d))?e:i[b];if(f=typeof c,"string"===f&&(e=Qb.exec(c))&&(c=(e[1]+1)*e[2]+parseFloat(m.css(a,b)),f="number"),null!=c&&c===c&&("number"!==f||m.cssNumber[h]||(c+="px"),k.clearCloneStyle||""!==c||0!==b.indexOf("background")||(i[b]="inherit"),!(g&&"set"in g&&void 0===(c=g.set(a,c,d)))))try{i[b]=c}catch(j){}}},css:function(a,b,c,d){var e,f,g,h=m.camelCase(b);return b=m.cssProps[h]||(m.cssProps[h]=Ub(a.style,h)),g=m.cssHooks[b]||m.cssHooks[h],g&&"get"in g&&(f=g.get(a,!0,c)),void 0===f&&(f=Jb(a,b,d)),"normal"===f&&b in Sb&&(f=Sb[b]),""===c||c?(e=parseFloat(f),c===!0||m.isNumeric(e)?e||0:f):f}}),m.each(["height","width"],function(a,b){m.cssHooks[b]={get:function(a,c,d){return c?Ob.test(m.css(a,"display"))&&0===a.offsetWidth?m.swap(a,Rb,function(){return Yb(a,b,d)}):Yb(a,b,d):void 0},set:function(a,c,d){var e=d&&Ib(a);return Wb(a,c,d?Xb(a,b,d,k.boxSizing&&"border-box"===m.css(a,"boxSizing",!1,e),e):0)}}}),k.opacity||(m.cssHooks.opacity={get:function(a,b){return Nb.test((b&&a.currentStyle?a.currentStyle.filter:a.style.filter)||"")?.01*parseFloat(RegExp.$1)+"":b?"1":""},set:function(a,b){var c=a.style,d=a.currentStyle,e=m.isNumeric(b)?"alpha(opacity="+100*b+")":"",f=d&&d.filter||c.filter||"";c.zoom=1,(b>=1||""===b)&&""===m.trim(f.replace(Mb,""))&&c.removeAttribute&&(c.removeAttribute("filter"),""===b||d&&!d.filter)||(c.filter=Mb.test(f)?f.replace(Mb,e):f+" "+e)}}),m.cssHooks.marginRight=Lb(k.reliableMarginRight,function(a,b){return b?m.swap(a,{display:"inline-block"},Jb,[a,"marginRight"]):void 0}),m.each({margin:"",padding:"",border:"Width"},function(a,b){m.cssHooks[a+b]={expand:function(c){for(var d=0,e={},f="string"==typeof c?c.split(" "):[c];4>d;d++)e[a+T[d]+b]=f[d]||f[d-2]||f[0];return e}},Gb.test(a)||(m.cssHooks[a+b].set=Wb)}),m.fn.extend({css:function(a,b){return V(this,function(a,b,c){var d,e,f={},g=0;if(m.isArray(b)){for(d=Ib(a),e=b.length;e>g;g++)f[b[g]]=m.css(a,b[g],!1,d);return f}return void 0!==c?m.style(a,b,c):m.css(a,b)},a,b,arguments.length>1)},show:function(){return Vb(this,!0)},hide:function(){return Vb(this)},toggle:function(a){return"boolean"==typeof a?a?this.show():this.hide():this.each(function(){U(this)?m(this).show():m(this).hide()})}});function Zb(a,b,c,d,e){return new Zb.prototype.init(a,b,c,d,e)}m.Tween=Zb,Zb.prototype={constructor:Zb,init:function(a,b,c,d,e,f){this.elem=a,this.prop=c,this.easing=e||"swing",this.options=b,this.start=this.now=this.cur(),this.end=d,this.unit=f||(m.cssNumber[c]?"":"px")
},cur:function(){var a=Zb.propHooks[this.prop];return a&&a.get?a.get(this):Zb.propHooks._default.get(this)},run:function(a){var b,c=Zb.propHooks[this.prop];return this.pos=b=this.options.duration?m.easing[this.easing](a,this.options.duration*a,0,1,this.options.duration):a,this.now=(this.end-this.start)*b+this.start,this.options.step&&this.options.step.call(this.elem,this.now,this),c&&c.set?c.set(this):Zb.propHooks._default.set(this),this}},Zb.prototype.init.prototype=Zb.prototype,Zb.propHooks={_default:{get:function(a){var b;return null==a.elem[a.prop]||a.elem.style&&null!=a.elem.style[a.prop]?(b=m.css(a.elem,a.prop,""),b&&"auto"!==b?b:0):a.elem[a.prop]},set:function(a){m.fx.step[a.prop]?m.fx.step[a.prop](a):a.elem.style&&(null!=a.elem.style[m.cssProps[a.prop]]||m.cssHooks[a.prop])?m.style(a.elem,a.prop,a.now+a.unit):a.elem[a.prop]=a.now}}},Zb.propHooks.scrollTop=Zb.propHooks.scrollLeft={set:function(a){a.elem.nodeType&&a.elem.parentNode&&(a.elem[a.prop]=a.now)}},m.easing={linear:function(a){return a},swing:function(a){return.5-Math.cos(a*Math.PI)/2}},m.fx=Zb.prototype.init,m.fx.step={};var $b,_b,ac=/^(?:toggle|show|hide)$/,bc=new RegExp("^(?:([+-])=|)("+S+")([a-z%]*)$","i"),cc=/queueHooks$/,dc=[ic],ec={"*":[function(a,b){var c=this.createTween(a,b),d=c.cur(),e=bc.exec(b),f=e&&e[3]||(m.cssNumber[a]?"":"px"),g=(m.cssNumber[a]||"px"!==f&&+d)&&bc.exec(m.css(c.elem,a)),h=1,i=20;if(g&&g[3]!==f){f=f||g[3],e=e||[],g=+d||1;do h=h||".5",g/=h,m.style(c.elem,a,g+f);while(h!==(h=c.cur()/d)&&1!==h&&--i)}return e&&(g=c.start=+g||+d||0,c.unit=f,c.end=e[1]?g+(e[1]+1)*e[2]:+e[2]),c}]};function fc(){return setTimeout(function(){$b=void 0}),$b=m.now()}function gc(a,b){var c,d={height:a},e=0;for(b=b?1:0;4>e;e+=2-b)c=T[e],d["margin"+c]=d["padding"+c]=a;return b&&(d.opacity=d.width=a),d}function hc(a,b,c){for(var d,e=(ec[b]||[]).concat(ec["*"]),f=0,g=e.length;g>f;f++)if(d=e[f].call(c,b,a))return d}function ic(a,b,c){var d,e,f,g,h,i,j,l,n=this,o={},p=a.style,q=a.nodeType&&U(a),r=m._data(a,"fxshow");c.queue||(h=m._queueHooks(a,"fx"),null==h.unqueued&&(h.unqueued=0,i=h.empty.fire,h.empty.fire=function(){h.unqueued||i()}),h.unqueued++,n.always(function(){n.always(function(){h.unqueued--,m.queue(a,"fx").length||h.empty.fire()})})),1===a.nodeType&&("height"in b||"width"in b)&&(c.overflow=[p.overflow,p.overflowX,p.overflowY],j=m.css(a,"display"),l="none"===j?m._data(a,"olddisplay")||Fb(a.nodeName):j,"inline"===l&&"none"===m.css(a,"float")&&(k.inlineBlockNeedsLayout&&"inline"!==Fb(a.nodeName)?p.zoom=1:p.display="inline-block")),c.overflow&&(p.overflow="hidden",k.shrinkWrapBlocks()||n.always(function(){p.overflow=c.overflow[0],p.overflowX=c.overflow[1],p.overflowY=c.overflow[2]}));for(d in b)if(e=b[d],ac.exec(e)){if(delete b[d],f=f||"toggle"===e,e===(q?"hide":"show")){if("show"!==e||!r||void 0===r[d])continue;q=!0}o[d]=r&&r[d]||m.style(a,d)}else j=void 0;if(m.isEmptyObject(o))"inline"===("none"===j?Fb(a.nodeName):j)&&(p.display=j);else{r?"hidden"in r&&(q=r.hidden):r=m._data(a,"fxshow",{}),f&&(r.hidden=!q),q?m(a).show():n.done(function(){m(a).hide()}),n.done(function(){var b;m._removeData(a,"fxshow");for(b in o)m.style(a,b,o[b])});for(d in o)g=hc(q?r[d]:0,d,n),d in r||(r[d]=g.start,q&&(g.end=g.start,g.start="width"===d||"height"===d?1:0))}}function jc(a,b){var c,d,e,f,g;for(c in a)if(d=m.camelCase(c),e=b[d],f=a[c],m.isArray(f)&&(e=f[1],f=a[c]=f[0]),c!==d&&(a[d]=f,delete a[c]),g=m.cssHooks[d],g&&"expand"in g){f=g.expand(f),delete a[d];for(c in f)c in a||(a[c]=f[c],b[c]=e)}else b[d]=e}function kc(a,b,c){var d,e,f=0,g=dc.length,h=m.Deferred().always(function(){delete i.elem}),i=function(){if(e)return!1;for(var b=$b||fc(),c=Math.max(0,j.startTime+j.duration-b),d=c/j.duration||0,f=1-d,g=0,i=j.tweens.length;i>g;g++)j.tweens[g].run(f);return h.notifyWith(a,[j,f,c]),1>f&&i?c:(h.resolveWith(a,[j]),!1)},j=h.promise({elem:a,props:m.extend({},b),opts:m.extend(!0,{specialEasing:{}},c),originalProperties:b,originalOptions:c,startTime:$b||fc(),duration:c.duration,tweens:[],createTween:function(b,c){var d=m.Tween(a,j.opts,b,c,j.opts.specialEasing[b]||j.opts.easing);return j.tweens.push(d),d},stop:function(b){var c=0,d=b?j.tweens.length:0;if(e)return this;for(e=!0;d>c;c++)j.tweens[c].run(1);return b?h.resolveWith(a,[j,b]):h.rejectWith(a,[j,b]),this}}),k=j.props;for(jc(k,j.opts.specialEasing);g>f;f++)if(d=dc[f].call(j,a,k,j.opts))return d;return m.map(k,hc,j),m.isFunction(j.opts.start)&&j.opts.start.call(a,j),m.fx.timer(m.extend(i,{elem:a,anim:j,queue:j.opts.queue})),j.progress(j.opts.progress).done(j.opts.done,j.opts.complete).fail(j.opts.fail).always(j.opts.always)}m.Animation=m.extend(kc,{tweener:function(a,b){m.isFunction(a)?(b=a,a=["*"]):a=a.split(" ");for(var c,d=0,e=a.length;e>d;d++)c=a[d],ec[c]=ec[c]||[],ec[c].unshift(b)},prefilter:function(a,b){b?dc.unshift(a):dc.push(a)}}),m.speed=function(a,b,c){var d=a&&"object"==typeof a?m.extend({},a):{complete:c||!c&&b||m.isFunction(a)&&a,duration:a,easing:c&&b||b&&!m.isFunction(b)&&b};return d.duration=m.fx.off?0:"number"==typeof d.duration?d.duration:d.duration in m.fx.speeds?m.fx.speeds[d.duration]:m.fx.speeds._default,(null==d.queue||d.queue===!0)&&(d.queue="fx"),d.old=d.complete,d.complete=function(){m.isFunction(d.old)&&d.old.call(this),d.queue&&m.dequeue(this,d.queue)},d},m.fn.extend({fadeTo:function(a,b,c,d){return this.filter(U).css("opacity",0).show().end().animate({opacity:b},a,c,d)},animate:function(a,b,c,d){var e=m.isEmptyObject(a),f=m.speed(b,c,d),g=function(){var b=kc(this,m.extend({},a),f);(e||m._data(this,"finish"))&&b.stop(!0)};return g.finish=g,e||f.queue===!1?this.each(g):this.queue(f.queue,g)},stop:function(a,b,c){var d=function(a){var b=a.stop;delete a.stop,b(c)};return"string"!=typeof a&&(c=b,b=a,a=void 0),b&&a!==!1&&this.queue(a||"fx",[]),this.each(function(){var b=!0,e=null!=a&&a+"queueHooks",f=m.timers,g=m._data(this);if(e)g[e]&&g[e].stop&&d(g[e]);else for(e in g)g[e]&&g[e].stop&&cc.test(e)&&d(g[e]);for(e=f.length;e--;)f[e].elem!==this||null!=a&&f[e].queue!==a||(f[e].anim.stop(c),b=!1,f.splice(e,1));(b||!c)&&m.dequeue(this,a)})},finish:function(a){return a!==!1&&(a=a||"fx"),this.each(function(){var b,c=m._data(this),d=c[a+"queue"],e=c[a+"queueHooks"],f=m.timers,g=d?d.length:0;for(c.finish=!0,m.queue(this,a,[]),e&&e.stop&&e.stop.call(this,!0),b=f.length;b--;)f[b].elem===this&&f[b].queue===a&&(f[b].anim.stop(!0),f.splice(b,1));for(b=0;g>b;b++)d[b]&&d[b].finish&&d[b].finish.call(this);delete c.finish})}}),m.each(["toggle","show","hide"],function(a,b){var c=m.fn[b];m.fn[b]=function(a,d,e){return null==a||"boolean"==typeof a?c.apply(this,arguments):this.animate(gc(b,!0),a,d,e)}}),m.each({slideDown:gc("show"),slideUp:gc("hide"),slideToggle:gc("toggle"),fadeIn:{opacity:"show"},fadeOut:{opacity:"hide"},fadeToggle:{opacity:"toggle"}},function(a,b){m.fn[a]=function(a,c,d){return this.animate(b,a,c,d)}}),m.timers=[],m.fx.tick=function(){var a,b=m.timers,c=0;for($b=m.now();c<b.length;c++)a=b[c],a()||b[c]!==a||b.splice(c--,1);b.length||m.fx.stop(),$b=void 0},m.fx.timer=function(a){m.timers.push(a),a()?m.fx.start():m.timers.pop()},m.fx.interval=13,m.fx.start=function(){_b||(_b=setInterval(m.fx.tick,m.fx.interval))},m.fx.stop=function(){clearInterval(_b),_b=null},m.fx.speeds={slow:600,fast:200,_default:400},m.fn.delay=function(a,b){return a=m.fx?m.fx.speeds[a]||a:a,b=b||"fx",this.queue(b,function(b,c){var d=setTimeout(b,a);c.stop=function(){clearTimeout(d)}})},function(){var a,b,c,d,e;b=y.createElement("div"),b.setAttribute("className","t"),b.innerHTML="  <link/><table></table><a href='/a'>a</a><input type='checkbox'/>",d=b.getElementsByTagName("a")[0],c=y.createElement("select"),e=c.appendChild(y.createElement("option")),a=b.getElementsByTagName("input")[0],d.style.cssText="top:1px",k.getSetAttribute="t"!==b.className,k.style=/top/.test(d.getAttribute("style")),k.hrefNormalized="/a"===d.getAttribute("href"),k.checkOn=!!a.value,k.optSelected=e.selected,k.enctype=!!y.createElement("form").enctype,c.disabled=!0,k.optDisabled=!e.disabled,a=y.createElement("input"),a.setAttribute("value",""),k.input=""===a.getAttribute("value"),a.value="t",a.setAttribute("type","radio"),k.radioValue="t"===a.value}();var lc=/\r/g;m.fn.extend({val:function(a){var b,c,d,e=this[0];{if(arguments.length)return d=m.isFunction(a),this.each(function(c){var e;1===this.nodeType&&(e=d?a.call(this,c,m(this).val()):a,null==e?e="":"number"==typeof e?e+="":m.isArray(e)&&(e=m.map(e,function(a){return null==a?"":a+""})),b=m.valHooks[this.type]||m.valHooks[this.nodeName.toLowerCase()],b&&"set"in b&&void 0!==b.set(this,e,"value")||(this.value=e))});if(e)return b=m.valHooks[e.type]||m.valHooks[e.nodeName.toLowerCase()],b&&"get"in b&&void 0!==(c=b.get(e,"value"))?c:(c=e.value,"string"==typeof c?c.replace(lc,""):null==c?"":c)}}}),m.extend({valHooks:{option:{get:function(a){var b=m.find.attr(a,"value");return null!=b?b:m.trim(m.text(a))}},select:{get:function(a){for(var b,c,d=a.options,e=a.selectedIndex,f="select-one"===a.type||0>e,g=f?null:[],h=f?e+1:d.length,i=0>e?h:f?e:0;h>i;i++)if(c=d[i],!(!c.selected&&i!==e||(k.optDisabled?c.disabled:null!==c.getAttribute("disabled"))||c.parentNode.disabled&&m.nodeName(c.parentNode,"optgroup"))){if(b=m(c).val(),f)return b;g.push(b)}return g},set:function(a,b){var c,d,e=a.options,f=m.makeArray(b),g=e.length;while(g--)if(d=e[g],m.inArray(m.valHooks.option.get(d),f)>=0)try{d.selected=c=!0}catch(h){d.scrollHeight}else d.selected=!1;return c||(a.selectedIndex=-1),e}}}}),m.each(["radio","checkbox"],function(){m.valHooks[this]={set:function(a,b){return m.isArray(b)?a.checked=m.inArray(m(a).val(),b)>=0:void 0}},k.checkOn||(m.valHooks[this].get=function(a){return null===a.getAttribute("value")?"on":a.value})});var mc,nc,oc=m.expr.attrHandle,pc=/^(?:checked|selected)$/i,qc=k.getSetAttribute,rc=k.input;m.fn.extend({attr:function(a,b){return V(this,m.attr,a,b,arguments.length>1)},removeAttr:function(a){return this.each(function(){m.removeAttr(this,a)})}}),m.extend({attr:function(a,b,c){var d,e,f=a.nodeType;if(a&&3!==f&&8!==f&&2!==f)return typeof a.getAttribute===K?m.prop(a,b,c):(1===f&&m.isXMLDoc(a)||(b=b.toLowerCase(),d=m.attrHooks[b]||(m.expr.match.bool.test(b)?nc:mc)),void 0===c?d&&"get"in d&&null!==(e=d.get(a,b))?e:(e=m.find.attr(a,b),null==e?void 0:e):null!==c?d&&"set"in d&&void 0!==(e=d.set(a,c,b))?e:(a.setAttribute(b,c+""),c):void m.removeAttr(a,b))},removeAttr:function(a,b){var c,d,e=0,f=b&&b.match(E);if(f&&1===a.nodeType)while(c=f[e++])d=m.propFix[c]||c,m.expr.match.bool.test(c)?rc&&qc||!pc.test(c)?a[d]=!1:a[m.camelCase("default-"+c)]=a[d]=!1:m.attr(a,c,""),a.removeAttribute(qc?c:d)},attrHooks:{type:{set:function(a,b){if(!k.radioValue&&"radio"===b&&m.nodeName(a,"input")){var c=a.value;return a.setAttribute("type",b),c&&(a.value=c),b}}}}}),nc={set:function(a,b,c){return b===!1?m.removeAttr(a,c):rc&&qc||!pc.test(c)?a.setAttribute(!qc&&m.propFix[c]||c,c):a[m.camelCase("default-"+c)]=a[c]=!0,c}},m.each(m.expr.match.bool.source.match(/\w+/g),function(a,b){var c=oc[b]||m.find.attr;oc[b]=rc&&qc||!pc.test(b)?function(a,b,d){var e,f;return d||(f=oc[b],oc[b]=e,e=null!=c(a,b,d)?b.toLowerCase():null,oc[b]=f),e}:function(a,b,c){return c?void 0:a[m.camelCase("default-"+b)]?b.toLowerCase():null}}),rc&&qc||(m.attrHooks.value={set:function(a,b,c){return m.nodeName(a,"input")?void(a.defaultValue=b):mc&&mc.set(a,b,c)}}),qc||(mc={set:function(a,b,c){var d=a.getAttributeNode(c);return d||a.setAttributeNode(d=a.ownerDocument.createAttribute(c)),d.value=b+="","value"===c||b===a.getAttribute(c)?b:void 0}},oc.id=oc.name=oc.coords=function(a,b,c){var d;return c?void 0:(d=a.getAttributeNode(b))&&""!==d.value?d.value:null},m.valHooks.button={get:function(a,b){var c=a.getAttributeNode(b);return c&&c.specified?c.value:void 0},set:mc.set},m.attrHooks.contenteditable={set:function(a,b,c){mc.set(a,""===b?!1:b,c)}},m.each(["width","height"],function(a,b){m.attrHooks[b]={set:function(a,c){return""===c?(a.setAttribute(b,"auto"),c):void 0}}})),k.style||(m.attrHooks.style={get:function(a){return a.style.cssText||void 0},set:function(a,b){return a.style.cssText=b+""}});var sc=/^(?:input|select|textarea|button|object)$/i,tc=/^(?:a|area)$/i;m.fn.extend({prop:function(a,b){return V(this,m.prop,a,b,arguments.length>1)},removeProp:function(a){return a=m.propFix[a]||a,this.each(function(){try{this[a]=void 0,delete this[a]}catch(b){}})}}),m.extend({propFix:{"for":"htmlFor","class":"className"},prop:function(a,b,c){var d,e,f,g=a.nodeType;if(a&&3!==g&&8!==g&&2!==g)return f=1!==g||!m.isXMLDoc(a),f&&(b=m.propFix[b]||b,e=m.propHooks[b]),void 0!==c?e&&"set"in e&&void 0!==(d=e.set(a,c,b))?d:a[b]=c:e&&"get"in e&&null!==(d=e.get(a,b))?d:a[b]},propHooks:{tabIndex:{get:function(a){var b=m.find.attr(a,"tabindex");return b?parseInt(b,10):sc.test(a.nodeName)||tc.test(a.nodeName)&&a.href?0:-1}}}}),k.hrefNormalized||m.each(["href","src"],function(a,b){m.propHooks[b]={get:function(a){return a.getAttribute(b,4)}}}),k.optSelected||(m.propHooks.selected={get:function(a){var b=a.parentNode;return b&&(b.selectedIndex,b.parentNode&&b.parentNode.selectedIndex),null}}),m.each(["tabIndex","readOnly","maxLength","cellSpacing","cellPadding","rowSpan","colSpan","useMap","frameBorder","contentEditable"],function(){m.propFix[this.toLowerCase()]=this}),k.enctype||(m.propFix.enctype="encoding");var uc=/[\t\r\n\f]/g;m.fn.extend({addClass:function(a){var b,c,d,e,f,g,h=0,i=this.length,j="string"==typeof a&&a;if(m.isFunction(a))return this.each(function(b){m(this).addClass(a.call(this,b,this.className))});if(j)for(b=(a||"").match(E)||[];i>h;h++)if(c=this[h],d=1===c.nodeType&&(c.className?(" "+c.className+" ").replace(uc," "):" ")){f=0;while(e=b[f++])d.indexOf(" "+e+" ")<0&&(d+=e+" ");g=m.trim(d),c.className!==g&&(c.className=g)}return this},removeClass:function(a){var b,c,d,e,f,g,h=0,i=this.length,j=0===arguments.length||"string"==typeof a&&a;if(m.isFunction(a))return this.each(function(b){m(this).removeClass(a.call(this,b,this.className))});if(j)for(b=(a||"").match(E)||[];i>h;h++)if(c=this[h],d=1===c.nodeType&&(c.className?(" "+c.className+" ").replace(uc," "):"")){f=0;while(e=b[f++])while(d.indexOf(" "+e+" ")>=0)d=d.replace(" "+e+" "," ");g=a?m.trim(d):"",c.className!==g&&(c.className=g)}return this},toggleClass:function(a,b){var c=typeof a;return"boolean"==typeof b&&"string"===c?b?this.addClass(a):this.removeClass(a):this.each(m.isFunction(a)?function(c){m(this).toggleClass(a.call(this,c,this.className,b),b)}:function(){if("string"===c){var b,d=0,e=m(this),f=a.match(E)||[];while(b=f[d++])e.hasClass(b)?e.removeClass(b):e.addClass(b)}else(c===K||"boolean"===c)&&(this.className&&m._data(this,"__className__",this.className),this.className=this.className||a===!1?"":m._data(this,"__className__")||"")})},hasClass:function(a){for(var b=" "+a+" ",c=0,d=this.length;d>c;c++)if(1===this[c].nodeType&&(" "+this[c].className+" ").replace(uc," ").indexOf(b)>=0)return!0;return!1}}),m.each("blur focus focusin focusout load resize scroll unload click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup error contextmenu".split(" "),function(a,b){m.fn[b]=function(a,c){return arguments.length>0?this.on(b,null,a,c):this.trigger(b)}}),m.fn.extend({hover:function(a,b){return this.mouseenter(a).mouseleave(b||a)},bind:function(a,b,c){return this.on(a,null,b,c)},unbind:function(a,b){return this.off(a,null,b)},delegate:function(a,b,c,d){return this.on(b,a,c,d)},undelegate:function(a,b,c){return 1===arguments.length?this.off(a,"**"):this.off(b,a||"**",c)}});var vc=m.now(),wc=/\?/,xc=/(,)|(\[|{)|(}|])|"(?:[^"\\\r\n]|\\["\\\/bfnrt]|\\u[\da-fA-F]{4})*"\s*:?|true|false|null|-?(?!0\d)\d+(?:\.\d+|)(?:[eE][+-]?\d+|)/g;m.parseJSON=function(b){if(a.JSON&&a.JSON.parse)return a.JSON.parse(b+"");var c,d=null,e=m.trim(b+"");return e&&!m.trim(e.replace(xc,function(a,b,e,f){return c&&b&&(d=0),0===d?a:(c=e||b,d+=!f-!e,"")}))?Function("return "+e)():m.error("Invalid JSON: "+b)},m.parseXML=function(b){var c,d;if(!b||"string"!=typeof b)return null;try{a.DOMParser?(d=new DOMParser,c=d.parseFromString(b,"text/xml")):(c=new ActiveXObject("Microsoft.XMLDOM"),c.async="false",c.loadXML(b))}catch(e){c=void 0}return c&&c.documentElement&&!c.getElementsByTagName("parsererror").length||m.error("Invalid XML: "+b),c};var yc,zc,Ac=/#.*$/,Bc=/([?&])_=[^&]*/,Cc=/^(.*?):[ \t]*([^\r\n]*)\r?$/gm,Dc=/^(?:about|app|app-storage|.+-extension|file|res|widget):$/,Ec=/^(?:GET|HEAD)$/,Fc=/^\/\//,Gc=/^([\w.+-]+:)(?:\/\/(?:[^\/?#]*@|)([^\/?#:]*)(?::(\d+)|)|)/,Hc={},Ic={},Jc="*/".concat("*");try{zc=location.href}catch(Kc){zc=y.createElement("a"),zc.href="",zc=zc.href}yc=Gc.exec(zc.toLowerCase())||[];function Lc(a){return function(b,c){"string"!=typeof b&&(c=b,b="*");var d,e=0,f=b.toLowerCase().match(E)||[];if(m.isFunction(c))while(d=f[e++])"+"===d.charAt(0)?(d=d.slice(1)||"*",(a[d]=a[d]||[]).unshift(c)):(a[d]=a[d]||[]).push(c)}}function Mc(a,b,c,d){var e={},f=a===Ic;function g(h){var i;return e[h]=!0,m.each(a[h]||[],function(a,h){var j=h(b,c,d);return"string"!=typeof j||f||e[j]?f?!(i=j):void 0:(b.dataTypes.unshift(j),g(j),!1)}),i}return g(b.dataTypes[0])||!e["*"]&&g("*")}function Nc(a,b){var c,d,e=m.ajaxSettings.flatOptions||{};for(d in b)void 0!==b[d]&&((e[d]?a:c||(c={}))[d]=b[d]);return c&&m.extend(!0,a,c),a}function Oc(a,b,c){var d,e,f,g,h=a.contents,i=a.dataTypes;while("*"===i[0])i.shift(),void 0===e&&(e=a.mimeType||b.getResponseHeader("Content-Type"));if(e)for(g in h)if(h[g]&&h[g].test(e)){i.unshift(g);break}if(i[0]in c)f=i[0];else{for(g in c){if(!i[0]||a.converters[g+" "+i[0]]){f=g;break}d||(d=g)}f=f||d}return f?(f!==i[0]&&i.unshift(f),c[f]):void 0}function Pc(a,b,c,d){var e,f,g,h,i,j={},k=a.dataTypes.slice();if(k[1])for(g in a.converters)j[g.toLowerCase()]=a.converters[g];f=k.shift();while(f)if(a.responseFields[f]&&(c[a.responseFields[f]]=b),!i&&d&&a.dataFilter&&(b=a.dataFilter(b,a.dataType)),i=f,f=k.shift())if("*"===f)f=i;else if("*"!==i&&i!==f){if(g=j[i+" "+f]||j["* "+f],!g)for(e in j)if(h=e.split(" "),h[1]===f&&(g=j[i+" "+h[0]]||j["* "+h[0]])){g===!0?g=j[e]:j[e]!==!0&&(f=h[0],k.unshift(h[1]));break}if(g!==!0)if(g&&a["throws"])b=g(b);else try{b=g(b)}catch(l){return{state:"parsererror",error:g?l:"No conversion from "+i+" to "+f}}}return{state:"success",data:b}}m.extend({active:0,lastModified:{},etag:{},ajaxSettings:{url:zc,type:"GET",isLocal:Dc.test(yc[1]),global:!0,processData:!0,async:!0,contentType:"application/x-www-form-urlencoded; charset=UTF-8",accepts:{"*":Jc,text:"text/plain",html:"text/html",xml:"application/xml, text/xml",json:"application/json, text/javascript"},contents:{xml:/xml/,html:/html/,json:/json/},responseFields:{xml:"responseXML",text:"responseText",json:"responseJSON"},converters:{"* text":String,"text html":!0,"text json":m.parseJSON,"text xml":m.parseXML},flatOptions:{url:!0,context:!0}},ajaxSetup:function(a,b){return b?Nc(Nc(a,m.ajaxSettings),b):Nc(m.ajaxSettings,a)},ajaxPrefilter:Lc(Hc),ajaxTransport:Lc(Ic),ajax:function(a,b){"object"==typeof a&&(b=a,a=void 0),b=b||{};var c,d,e,f,g,h,i,j,k=m.ajaxSetup({},b),l=k.context||k,n=k.context&&(l.nodeType||l.jquery)?m(l):m.event,o=m.Deferred(),p=m.Callbacks("once memory"),q=k.statusCode||{},r={},s={},t=0,u="canceled",v={readyState:0,getResponseHeader:function(a){var b;if(2===t){if(!j){j={};while(b=Cc.exec(f))j[b[1].toLowerCase()]=b[2]}b=j[a.toLowerCase()]}return null==b?null:b},getAllResponseHeaders:function(){return 2===t?f:null},setRequestHeader:function(a,b){var c=a.toLowerCase();return t||(a=s[c]=s[c]||a,r[a]=b),this},overrideMimeType:function(a){return t||(k.mimeType=a),this},statusCode:function(a){var b;if(a)if(2>t)for(b in a)q[b]=[q[b],a[b]];else v.always(a[v.status]);return this},abort:function(a){var b=a||u;return i&&i.abort(b),x(0,b),this}};if(o.promise(v).complete=p.add,v.success=v.done,v.error=v.fail,k.url=((a||k.url||zc)+"").replace(Ac,"").replace(Fc,yc[1]+"//"),k.type=b.method||b.type||k.method||k.type,k.dataTypes=m.trim(k.dataType||"*").toLowerCase().match(E)||[""],null==k.crossDomain&&(c=Gc.exec(k.url.toLowerCase()),k.crossDomain=!(!c||c[1]===yc[1]&&c[2]===yc[2]&&(c[3]||("http:"===c[1]?"80":"443"))===(yc[3]||("http:"===yc[1]?"80":"443")))),k.data&&k.processData&&"string"!=typeof k.data&&(k.data=m.param(k.data,k.traditional)),Mc(Hc,k,b,v),2===t)return v;h=k.global,h&&0===m.active++&&m.event.trigger("ajaxStart"),k.type=k.type.toUpperCase(),k.hasContent=!Ec.test(k.type),e=k.url,k.hasContent||(k.data&&(e=k.url+=(wc.test(e)?"&":"?")+k.data,delete k.data),k.cache===!1&&(k.url=Bc.test(e)?e.replace(Bc,"$1_="+vc++):e+(wc.test(e)?"&":"?")+"_="+vc++)),k.ifModified&&(m.lastModified[e]&&v.setRequestHeader("If-Modified-Since",m.lastModified[e]),m.etag[e]&&v.setRequestHeader("If-None-Match",m.etag[e])),(k.data&&k.hasContent&&k.contentType!==!1||b.contentType)&&v.setRequestHeader("Content-Type",k.contentType),v.setRequestHeader("Accept",k.dataTypes[0]&&k.accepts[k.dataTypes[0]]?k.accepts[k.dataTypes[0]]+("*"!==k.dataTypes[0]?", "+Jc+"; q=0.01":""):k.accepts["*"]);for(d in k.headers)v.setRequestHeader(d,k.headers[d]);if(k.beforeSend&&(k.beforeSend.call(l,v,k)===!1||2===t))return v.abort();u="abort";for(d in{success:1,error:1,complete:1})v[d](k[d]);if(i=Mc(Ic,k,b,v)){v.readyState=1,h&&n.trigger("ajaxSend",[v,k]),k.async&&k.timeout>0&&(g=setTimeout(function(){v.abort("timeout")},k.timeout));try{t=1,i.send(r,x)}catch(w){if(!(2>t))throw w;x(-1,w)}}else x(-1,"No Transport");function x(a,b,c,d){var j,r,s,u,w,x=b;2!==t&&(t=2,g&&clearTimeout(g),i=void 0,f=d||"",v.readyState=a>0?4:0,j=a>=200&&300>a||304===a,c&&(u=Oc(k,v,c)),u=Pc(k,u,v,j),j?(k.ifModified&&(w=v.getResponseHeader("Last-Modified"),w&&(m.lastModified[e]=w),w=v.getResponseHeader("etag"),w&&(m.etag[e]=w)),204===a||"HEAD"===k.type?x="nocontent":304===a?x="notmodified":(x=u.state,r=u.data,s=u.error,j=!s)):(s=x,(a||!x)&&(x="error",0>a&&(a=0))),v.status=a,v.statusText=(b||x)+"",j?o.resolveWith(l,[r,x,v]):o.rejectWith(l,[v,x,s]),v.statusCode(q),q=void 0,h&&n.trigger(j?"ajaxSuccess":"ajaxError",[v,k,j?r:s]),p.fireWith(l,[v,x]),h&&(n.trigger("ajaxComplete",[v,k]),--m.active||m.event.trigger("ajaxStop")))}return v},getJSON:function(a,b,c){return m.get(a,b,c,"json")},getScript:function(a,b){return m.get(a,void 0,b,"script")}}),m.each(["get","post"],function(a,b){m[b]=function(a,c,d,e){return m.isFunction(c)&&(e=e||d,d=c,c=void 0),m.ajax({url:a,type:b,dataType:e,data:c,success:d})}}),m.each(["ajaxStart","ajaxStop","ajaxComplete","ajaxError","ajaxSuccess","ajaxSend"],function(a,b){m.fn[b]=function(a){return this.on(b,a)}}),m._evalUrl=function(a){return m.ajax({url:a,type:"GET",dataType:"script",async:!1,global:!1,"throws":!0})},m.fn.extend({wrapAll:function(a){if(m.isFunction(a))return this.each(function(b){m(this).wrapAll(a.call(this,b))});if(this[0]){var b=m(a,this[0].ownerDocument).eq(0).clone(!0);this[0].parentNode&&b.insertBefore(this[0]),b.map(function(){var a=this;while(a.firstChild&&1===a.firstChild.nodeType)a=a.firstChild;return a}).append(this)}return this},wrapInner:function(a){return this.each(m.isFunction(a)?function(b){m(this).wrapInner(a.call(this,b))}:function(){var b=m(this),c=b.contents();c.length?c.wrapAll(a):b.append(a)})},wrap:function(a){var b=m.isFunction(a);return this.each(function(c){m(this).wrapAll(b?a.call(this,c):a)})},unwrap:function(){return this.parent().each(function(){m.nodeName(this,"body")||m(this).replaceWith(this.childNodes)}).end()}}),m.expr.filters.hidden=function(a){return a.offsetWidth<=0&&a.offsetHeight<=0||!k.reliableHiddenOffsets()&&"none"===(a.style&&a.style.display||m.css(a,"display"))},m.expr.filters.visible=function(a){return!m.expr.filters.hidden(a)};var Qc=/%20/g,Rc=/\[\]$/,Sc=/\r?\n/g,Tc=/^(?:submit|button|image|reset|file)$/i,Uc=/^(?:input|select|textarea|keygen)/i;function Vc(a,b,c,d){var e;if(m.isArray(b))m.each(b,function(b,e){c||Rc.test(a)?d(a,e):Vc(a+"["+("object"==typeof e?b:"")+"]",e,c,d)});else if(c||"object"!==m.type(b))d(a,b);else for(e in b)Vc(a+"["+e+"]",b[e],c,d)}m.param=function(a,b){var c,d=[],e=function(a,b){b=m.isFunction(b)?b():null==b?"":b,d[d.length]=encodeURIComponent(a)+"="+encodeURIComponent(b)};if(void 0===b&&(b=m.ajaxSettings&&m.ajaxSettings.traditional),m.isArray(a)||a.jquery&&!m.isPlainObject(a))m.each(a,function(){e(this.name,this.value)});else for(c in a)Vc(c,a[c],b,e);return d.join("&").replace(Qc,"+")},m.fn.extend({serialize:function(){return m.param(this.serializeArray())},serializeArray:function(){return this.map(function(){var a=m.prop(this,"elements");return a?m.makeArray(a):this}).filter(function(){var a=this.type;return this.name&&!m(this).is(":disabled")&&Uc.test(this.nodeName)&&!Tc.test(a)&&(this.checked||!W.test(a))}).map(function(a,b){var c=m(this).val();return null==c?null:m.isArray(c)?m.map(c,function(a){return{name:b.name,value:a.replace(Sc,"\r\n")}}):{name:b.name,value:c.replace(Sc,"\r\n")}}).get()}}),m.ajaxSettings.xhr=void 0!==a.ActiveXObject?function(){return!this.isLocal&&/^(get|post|head|put|delete|options)$/i.test(this.type)&&Zc()||$c()}:Zc;var Wc=0,Xc={},Yc=m.ajaxSettings.xhr();a.ActiveXObject&&m(a).on("unload",function(){for(var a in Xc)Xc[a](void 0,!0)}),k.cors=!!Yc&&"withCredentials"in Yc,Yc=k.ajax=!!Yc,Yc&&m.ajaxTransport(function(a){if(!a.crossDomain||k.cors){var b;return{send:function(c,d){var e,f=a.xhr(),g=++Wc;if(f.open(a.type,a.url,a.async,a.username,a.password),a.xhrFields)for(e in a.xhrFields)f[e]=a.xhrFields[e];a.mimeType&&f.overrideMimeType&&f.overrideMimeType(a.mimeType),a.crossDomain||c["X-Requested-With"]||(c["X-Requested-With"]="XMLHttpRequest");for(e in c)void 0!==c[e]&&f.setRequestHeader(e,c[e]+"");f.send(a.hasContent&&a.data||null),b=function(c,e){var h,i,j;if(b&&(e||4===f.readyState))if(delete Xc[g],b=void 0,f.onreadystatechange=m.noop,e)4!==f.readyState&&f.abort();else{j={},h=f.status,"string"==typeof f.responseText&&(j.text=f.responseText);try{i=f.statusText}catch(k){i=""}h||!a.isLocal||a.crossDomain?1223===h&&(h=204):h=j.text?200:404}j&&d(h,i,j,f.getAllResponseHeaders())},a.async?4===f.readyState?setTimeout(b):f.onreadystatechange=Xc[g]=b:b()},abort:function(){b&&b(void 0,!0)}}}});function Zc(){try{return new a.XMLHttpRequest}catch(b){}}function $c(){try{return new a.ActiveXObject("Microsoft.XMLHTTP")}catch(b){}}m.ajaxSetup({accepts:{script:"text/javascript, application/javascript, application/ecmascript, application/x-ecmascript"},contents:{script:/(?:java|ecma)script/},converters:{"text script":function(a){return m.globalEval(a),a}}}),m.ajaxPrefilter("script",function(a){void 0===a.cache&&(a.cache=!1),a.crossDomain&&(a.type="GET",a.global=!1)}),m.ajaxTransport("script",function(a){if(a.crossDomain){var b,c=y.head||m("head")[0]||y.documentElement;return{send:function(d,e){b=y.createElement("script"),b.async=!0,a.scriptCharset&&(b.charset=a.scriptCharset),b.src=a.url,b.onload=b.onreadystatechange=function(a,c){(c||!b.readyState||/loaded|complete/.test(b.readyState))&&(b.onload=b.onreadystatechange=null,b.parentNode&&b.parentNode.removeChild(b),b=null,c||e(200,"success"))},c.insertBefore(b,c.firstChild)},abort:function(){b&&b.onload(void 0,!0)}}}});var _c=[],ad=/(=)\?(?=&|$)|\?\?/;m.ajaxSetup({jsonp:"callback",jsonpCallback:function(){var a=_c.pop()||m.expando+"_"+vc++;return this[a]=!0,a}}),m.ajaxPrefilter("json jsonp",function(b,c,d){var e,f,g,h=b.jsonp!==!1&&(ad.test(b.url)?"url":"string"==typeof b.data&&!(b.contentType||"").indexOf("application/x-www-form-urlencoded")&&ad.test(b.data)&&"data");return h||"jsonp"===b.dataTypes[0]?(e=b.jsonpCallback=m.isFunction(b.jsonpCallback)?b.jsonpCallback():b.jsonpCallback,h?b[h]=b[h].replace(ad,"$1"+e):b.jsonp!==!1&&(b.url+=(wc.test(b.url)?"&":"?")+b.jsonp+"="+e),b.converters["script json"]=function(){return g||m.error(e+" was not called"),g[0]},b.dataTypes[0]="json",f=a[e],a[e]=function(){g=arguments},d.always(function(){a[e]=f,b[e]&&(b.jsonpCallback=c.jsonpCallback,_c.push(e)),g&&m.isFunction(f)&&f(g[0]),g=f=void 0}),"script"):void 0}),m.parseHTML=function(a,b,c){if(!a||"string"!=typeof a)return null;"boolean"==typeof b&&(c=b,b=!1),b=b||y;var d=u.exec(a),e=!c&&[];return d?[b.createElement(d[1])]:(d=m.buildFragment([a],b,e),e&&e.length&&m(e).remove(),m.merge([],d.childNodes))};var bd=m.fn.load;m.fn.load=function(a,b,c){if("string"!=typeof a&&bd)return bd.apply(this,arguments);var d,e,f,g=this,h=a.indexOf(" ");return h>=0&&(d=m.trim(a.slice(h,a.length)),a=a.slice(0,h)),m.isFunction(b)?(c=b,b=void 0):b&&"object"==typeof b&&(f="POST"),g.length>0&&m.ajax({url:a,type:f,dataType:"html",data:b}).done(function(a){e=arguments,g.html(d?m("<div>").append(m.parseHTML(a)).find(d):a)}).complete(c&&function(a,b){g.each(c,e||[a.responseText,b,a])}),this},m.expr.filters.animated=function(a){return m.grep(m.timers,function(b){return a===b.elem}).length};var cd=a.document.documentElement;function dd(a){return m.isWindow(a)?a:9===a.nodeType?a.defaultView||a.parentWindow:!1}m.offset={setOffset:function(a,b,c){var d,e,f,g,h,i,j,k=m.css(a,"position"),l=m(a),n={};"static"===k&&(a.style.position="relative"),h=l.offset(),f=m.css(a,"top"),i=m.css(a,"left"),j=("absolute"===k||"fixed"===k)&&m.inArray("auto",[f,i])>-1,j?(d=l.position(),g=d.top,e=d.left):(g=parseFloat(f)||0,e=parseFloat(i)||0),m.isFunction(b)&&(b=b.call(a,c,h)),null!=b.top&&(n.top=b.top-h.top+g),null!=b.left&&(n.left=b.left-h.left+e),"using"in b?b.using.call(a,n):l.css(n)}},m.fn.extend({offset:function(a){if(arguments.length)return void 0===a?this:this.each(function(b){m.offset.setOffset(this,a,b)});var b,c,d={top:0,left:0},e=this[0],f=e&&e.ownerDocument;if(f)return b=f.documentElement,m.contains(b,e)?(typeof e.getBoundingClientRect!==K&&(d=e.getBoundingClientRect()),c=dd(f),{top:d.top+(c.pageYOffset||b.scrollTop)-(b.clientTop||0),left:d.left+(c.pageXOffset||b.scrollLeft)-(b.clientLeft||0)}):d},position:function(){if(this[0]){var a,b,c={top:0,left:0},d=this[0];return"fixed"===m.css(d,"position")?b=d.getBoundingClientRect():(a=this.offsetParent(),b=this.offset(),m.nodeName(a[0],"html")||(c=a.offset()),c.top+=m.css(a[0],"borderTopWidth",!0),c.left+=m.css(a[0],"borderLeftWidth",!0)),{top:b.top-c.top-m.css(d,"marginTop",!0),left:b.left-c.left-m.css(d,"marginLeft",!0)}}},offsetParent:function(){return this.map(function(){var a=this.offsetParent||cd;while(a&&!m.nodeName(a,"html")&&"static"===m.css(a,"position"))a=a.offsetParent;return a||cd})}}),m.each({scrollLeft:"pageXOffset",scrollTop:"pageYOffset"},function(a,b){var c=/Y/.test(b);m.fn[a]=function(d){return V(this,function(a,d,e){var f=dd(a);return void 0===e?f?b in f?f[b]:f.document.documentElement[d]:a[d]:void(f?f.scrollTo(c?m(f).scrollLeft():e,c?e:m(f).scrollTop()):a[d]=e)},a,d,arguments.length,null)}}),m.each(["top","left"],function(a,b){m.cssHooks[b]=Lb(k.pixelPosition,function(a,c){return c?(c=Jb(a,b),Hb.test(c)?m(a).position()[b]+"px":c):void 0})}),m.each({Height:"height",Width:"width"},function(a,b){m.each({padding:"inner"+a,content:b,"":"outer"+a},function(c,d){m.fn[d]=function(d,e){var f=arguments.length&&(c||"boolean"!=typeof d),g=c||(d===!0||e===!0?"margin":"border");return V(this,function(b,c,d){var e;return m.isWindow(b)?b.document.documentElement["client"+a]:9===b.nodeType?(e=b.documentElement,Math.max(b.body["scroll"+a],e["scroll"+a],b.body["offset"+a],e["offset"+a],e["client"+a])):void 0===d?m.css(b,c,g):m.style(b,c,d,g)},b,f?d:void 0,f,null)}})}),m.fn.size=function(){return this.length},m.fn.andSelf=m.fn.addBack,"function"==typeof define&&define.amd&&define("jquery",[],function(){return m});var ed=a.jQuery,fd=a.$;return m.noConflict=function(b){return a.$===m&&(a.$=fd),b&&a.jQuery===m&&(a.jQuery=ed),m},typeof b===K&&(a.jQuery=a.$=m),m});
            //]]>
    </script>
    <script type='text/javascript'>
            //<![CDATA[
            /*!
 * The Final Countdown for jQuery v2.2.0 (http://hilios.github.io/jQuery.countdown/)
 */
!function(a){"use strict";"function"==typeof define&&define.amd?define(["jquery"],a):a(jQuery)}(function(a){"use strict";function b(a){if(a instanceof Date)return a;if(String(a).match(g))return String(a).match(/^[0-9]*$/)&&(a=Number(a)),String(a).match(/\-/)&&(a=String(a).replace(/\-/g,"/")),new Date(a);throw new Error("Couldn't cast `"+a+"` to a date object.")}function c(a){var b=a.toString().replace(/([.?*+^$[\]\\(){}|-])/g,"\\$1");return new RegExp(b)}function d(a){return function(b){var d=b.match(/%(-|!)?[A-Z]{1}(:[^;]+;)?/gi);if(d)for(var f=0,g=d.length;f<g;++f){var h=d[f].match(/%(-|!)?([a-zA-Z]{1})(:[^;]+;)?/),j=c(h[0]),k=h[1]||"",l=h[3]||"",m=null;h=h[2],i.hasOwnProperty(h)&&(m=i[h],m=Number(a[m])),null!==m&&("!"===k&&(m=e(l,m)),""===k&&m<10&&(m="0"+m.toString()),b=b.replace(j,m.toString()))}return b=b.replace(/%%/,"%")}}function e(a,b){var c="s",d="";return a&&(a=a.replace(/(:|;|\s)/gi,"").split(/\,/),1===a.length?c=a[0]:(d=a[0],c=a[1])),Math.abs(b)>1?c:d}var f=[],g=[],h={precision:100,elapse:!1,defer:!1};g.push(/^[0-9]*$/.source),g.push(/([0-9]{1,2}\/){2}[0-9]{4}( [0-9]{1,2}(:[0-9]{2}){2})?/.source),g.push(/[0-9]{4}([\/\-][0-9]{1,2}){2}( [0-9]{1,2}(:[0-9]{2}){2})?/.source),g=new RegExp(g.join("|"));var i={Y:"years",m:"months",n:"daysToMonth",d:"daysToWeek",w:"weeks",W:"weeksToMonth",H:"hours",M:"minutes",S:"seconds",D:"totalDays",I:"totalHours",N:"totalMinutes",T:"totalSeconds"},j=function(b,c,d){this.el=b,this.$el=a(b),this.interval=null,this.offset={},this.options=a.extend({},h),this.instanceNumber=f.length,f.push(this),this.$el.data("countdown-instance",this.instanceNumber),d&&("function"==typeof d?(this.$el.on("update.countdown",d),this.$el.on("stoped.countdown",d),this.$el.on("finish.countdown",d)):this.options=a.extend({},h,d)),this.setFinalDate(c),this.options.defer===!1&&this.start()};a.extend(j.prototype,{start:function(){null!==this.interval&&clearInterval(this.interval);var a=this;this.update(),this.interval=setInterval(function(){a.update.call(a)},this.options.precision)},stop:function(){clearInterval(this.interval),this.interval=null,this.dispatchEvent("stoped")},toggle:function(){this.interval?this.stop():this.start()},pause:function(){this.stop()},resume:function(){this.start()},remove:function(){this.stop.call(this),f[this.instanceNumber]=null,delete this.$el.data().countdownInstance},setFinalDate:function(a){this.finalDate=b(a)},update:function(){if(0===this.$el.closest("html").length)return void this.remove();var b,c=void 0!==a._data(this.el,"events"),d=new Date;b=this.finalDate.getTime()-d.getTime(),b=Math.ceil(b/1e3),b=!this.options.elapse&&b<0?0:Math.abs(b),this.totalSecsLeft!==b&&c&&(this.totalSecsLeft=b,this.elapsed=d>=this.finalDate,this.offset={seconds:this.totalSecsLeft%60,minutes:Math.floor(this.totalSecsLeft/60)%60,hours:Math.floor(this.totalSecsLeft/60/60)%24,days:Math.floor(this.totalSecsLeft/60/60/24)%7,daysToWeek:Math.floor(this.totalSecsLeft/60/60/24)%7,daysToMonth:Math.floor(this.totalSecsLeft/60/60/24%30.4368),weeks:Math.floor(this.totalSecsLeft/60/60/24/7),weeksToMonth:Math.floor(this.totalSecsLeft/60/60/24/7)%4,months:Math.floor(this.totalSecsLeft/60/60/24/30.4368),years:Math.abs(this.finalDate.getFullYear()-d.getFullYear()),totalDays:Math.floor(this.totalSecsLeft/60/60/24),totalHours:Math.floor(this.totalSecsLeft/60/60),totalMinutes:Math.floor(this.totalSecsLeft/60),totalSeconds:this.totalSecsLeft},this.options.elapse||0!==this.totalSecsLeft?this.dispatchEvent("update"):(this.stop(),this.dispatchEvent("finish")))},dispatchEvent:function(b){var c=a.Event(b+".countdown");c.finalDate=this.finalDate,c.elapsed=this.elapsed,c.offset=a.extend({},this.offset),c.strftime=d(this.offset),this.$el.trigger(c)}}),a.fn.countdown=function(){var b=Array.prototype.slice.call(arguments,0);return this.each(function(){var c=a(this).data("countdown-instance");if(void 0!==c){var d=f[c],e=b[0];j.prototype.hasOwnProperty(e)?d[e].apply(d,b.slice(1)):null===String(e).match(/^[$A-Z_][0-9A-Z_$]*$/i)?(d.setFinalDate.call(d,e),d.start()):a.error("Method %s does not exist on jQuery.countdown".replace(/\%s/gi,e))}else new j(this,b[0],b[1])})}});
            /*
	By AndrÃ© Rinas, www.andreknieriem.de
	Available for use under the MIT License
*/
!function(a,b,c,d){"use strict";a.fn.simpleLightbox=function(d){var t,d=a.extend({overlay:!0,spinner:!0,nav:!0,navText:["&lsaquo;","&rsaquo;"],captions:!0,captionDelay:0,captionSelector:"img",captionType:"attr",captionsData:"title",captionPosition:"bottom",close:!0,closeText:"X—",swipeClose:!0,showCounter:!0,fileExt:"png|jpg|jpeg|gif",animationSlide:!0,animationSpeed:250,preloading:!0,enableKeyboard:!0,loop:!0,rel:!1,docClose:!0,swipeTolerance:50,className:"simple-lightbox",widthRatio:.8,heightRatio:.9,disableRightClick:!1,disableScroll:!0,alertError:!0,alertErrorMessage:"Image not found, next image will be loaded",additionalHtml:!1,history:!0},d),h=(b.navigator.pointerEnabled||b.navigator.msPointerEnabled,0),i=0,j=a(),k=function(){var a=c.body||c.documentElement;return a=a.style,""===a.WebkitTransition?"-webkit-":""===a.MozTransition?"-moz-":""===a.OTransition?"-o-":""===a.transition&&""},l=!1,m=[],n=function(b,c){var d=a(c.selector).filter(function(){return a(this).attr("rel")===b});return d},o=d.rel&&d.rel!==!1?n(d.rel,this):this,k=k(),p=0,q=k!==!1,r="pushState"in history,s=!1,u=b.location,v=function(){return u.hash.substring(1)},w=v(),x=function(){var b=(v(),"pid="+(H+1)),d=u.href.split("#")[0]+"#"+b;r?history[s?"replaceState":"pushState"]("",c.title,d):s?u.replace(d):u.hash=b,s=!0},y=function(){r?history.pushState("",c.title,u.pathname+u.search):u.hash="",clearTimeout(t)},z=function(){s?t=setTimeout(x,800):x()},A="simplelb",B=a("<div>").addClass("sl-overlay"),C=a("<button>").addClass("sl-close").html(d.closeText),D=a("<div>").addClass("sl-spinner").html("<div></div>"),E=a("<div>").addClass("sl-navigation").html('<button class="sl-prev">'+d.navText[0]+'</button><button class="sl-next">'+d.navText[1]+"</button>"),F=a("<div>").addClass("sl-counter").html('<span class="sl-current"></span>/<span class="sl-total"></span>'),G=!1,H=0,I=a("<div>").addClass("sl-caption pos-"+d.captionPosition),J=a("<div>").addClass("sl-image"),K=a("<div>").addClass("sl-wrapper").addClass(d.className),L=function(b){return!d.fileExt||"a"==a(b).prop("tagName").toLowerCase()&&new RegExp(".("+d.fileExt+")$","i").test(a(b).attr("href"))},M=function(){d.close&&C.appendTo(K),d.showCounter&&o.length>1&&(F.appendTo(K),F.find(".sl-total").text(o.length)),d.nav&&E.appendTo(K),d.spinner&&D.appendTo(K)},N=function(b){b.trigger(a.Event("show.simplelightbox")),d.disableScroll&&(p=W("hide")),K.appendTo("body"),J.appendTo(K),d.overlay&&B.appendTo(a("body")),G=!0,H=o.index(b),j=a("<img/>").hide().attr("src",b.attr("href")),m.indexOf(b.attr("href"))==-1&&m.push(b.attr("href")),J.html("").attr("style",""),j.appendTo(J),R(),B.fadeIn("fast"),a(".sl-close").fadeIn("fast"),D.show(),E.fadeIn("fast"),a(".sl-wrapper .sl-counter .sl-current").text(H+1),F.fadeIn("fast"),O(),d.preloading&&T(),setTimeout(function(){b.trigger(a.Event("shown.simplelightbox"))},d.animationSpeed)},O=function(c){if(j.length){var e=new Image,f=a(b).width()*d.widthRatio,g=a(b).height()*d.heightRatio;e.src=j.attr("src"),a(e).bind("error",function(b){o.eq(H).trigger(a.Event("error.simplelightbox")),G=!1,l=!0,D.hide(),d.alertError&&alert(d.alertErrorMessage),U(1==c||c==-1?c:1)}),e.onload=function(){"undefined"!=typeof c&&o.eq(H).trigger(a.Event("changed.simplelightbox")).trigger(a.Event((1===c?"nextDone":"prevDone")+".simplelightbox")),d.history&&z(),m.indexOf(j.attr("src"))==-1&&m.push(j.attr("src"));var h=e.width,i=e.height;if(h>f||i>g){var k=h/i>f/g?h/f:i/g;h/=k,i/=k}a(".sl-image").css({top:(a(b).height()-i)/2+"px",left:(a(b).width()-h-p)/2+"px"}),D.hide(),j.css({width:h+"px",height:i+"px"}).fadeIn("fast"),l=!0;var r,n="self"==d.captionSelector?o.eq(H):o.eq(H).find(d.captionSelector);if(r="data"==d.captionType?n.data(d.captionsData):"text"==d.captionType?n.html():n.prop(d.captionsData),d.loop||(0===H&&a(".sl-prev").hide(),H>=o.length-1&&a(".sl-next").hide(),H>0&&a(".sl-prev").show(),H<o.length-1&&a(".sl-next").show()),1==o.length&&a(".sl-prev, .sl-next").hide(),1==c||c==-1){var s={opacity:1};d.animationSlide&&(q?(Q(0,100*c+"px"),setTimeout(function(){Q(d.animationSpeed/1e3,"0px"),50})):s.left=parseInt(a(".sl-image").css("left"))+100*c+"px"),a(".sl-image").animate(s,d.animationSpeed,function(){G=!1,P(r)})}else G=!1,P(r);d.additionalHtml&&0===a(".sl-additional-html").length&&a("<div>").html(d.additionalHtml).addClass("sl-additional-html").appendTo(a(".sl-image"))}}},P=function(b){""!==b&&"undefined"!=typeof b&&d.captions&&I.html(b).hide().appendTo(a(".sl-image")).delay(d.captionDelay).fadeIn("fast")},Q=function(b,c){var d={};d[k+"transform"]="translateX("+c+")",d[k+"transition"]=k+"transform "+b+"s linear",a(".sl-image").css(d)},R=function(){a(b).on("resize."+A,O),a(c).on("click."+A+" touchstart."+A,".sl-close",function(a){a.preventDefault(),l&&V()}),d.history&&setTimeout(function(){a(b).on("hashchange."+A,function(){if(l&&v()===w)return void V()})},40),E.on("click."+A,"button",function(b){b.preventDefault(),h=0,U(a(this).hasClass("sl-next")?1:-1)});var e=0,f=0,g=0,j=0,k=!1,m=0;J.on("touchstart."+A+" mousedown."+A,function(a){return!!k||(q&&(m=parseInt(J.css("left"))),k=!0,e=a.originalEvent.pageX||a.originalEvent.touches[0].pageX,g=a.originalEvent.pageY||a.originalEvent.touches[0].pageY,!1)}).on("touchmove."+A+" mousemove."+A+" pointermove MSPointerMove",function(a){return!k||(a.preventDefault(),f=a.originalEvent.pageX||a.originalEvent.touches[0].pageX,j=a.originalEvent.pageY||a.originalEvent.touches[0].pageY,h=e-f,i=g-j,void(d.animationSlide&&(q?Q(0,-h+"px"):J.css("left",m-h+"px"))))}).on("touchend."+A+" mouseup."+A+" touchcancel."+A+" mouseleave."+A+" pointerup pointercancel MSPointerUp MSPointerCancel",function(a){if(k){k=!1;var b=!0;d.loop||(0===H&&h<0&&(b=!1),H>=o.length-1&&h>0&&(b=!1)),Math.abs(h)>d.swipeTolerance&&b?U(h>0?1:-1):d.animationSlide&&(q?Q(d.animationSpeed/1e3,"0px"):J.animate({left:m+"px"},d.animationSpeed/2)),d.swipeClose&&Math.abs(i)>50&&Math.abs(h)<d.swipeTolerance&&V()}})},S=function(){E.off("click","button"),a(c).off("click."+A,".sl-close"),a(b).off("resize."+A),a(b).off("hashchange."+A)},T=function(){var b=H+1<0?o.length-1:H+1>=o.length-1?0:H+1,c=H-1<0?o.length-1:H-1>=o.length-1?0:H-1;a("<img />").attr("src",o.eq(b).attr("href")).on("load",function(){m.indexOf(a(this).attr("src"))==-1&&m.push(a(this).attr("src")),o.eq(H).trigger(a.Event("nextImageLoaded.simplelightbox"))}),a("<img />").attr("src",o.eq(c).attr("href")).on("load",function(){m.indexOf(a(this).attr("src"))==-1&&m.push(a(this).attr("src")),o.eq(H).trigger(a.Event("prevImageLoaded.simplelightbox"))})},U=function(b){o.eq(H).trigger(a.Event("change.simplelightbox")).trigger(a.Event((1===b?"next":"prev")+".simplelightbox"));var c=H+b;if(!(G||(c<0||c>=o.length)&&d.loop===!1)){H=c<0?o.length-1:c>o.length-1?0:c,a(".sl-wrapper .sl-counter .sl-current").text(H+1);var e={opacity:0};d.animationSlide&&(q?Q(d.animationSpeed/1e3,-100*b-h+"px"):e.left=parseInt(a(".sl-image").css("left"))+-100*b+"px"),a(".sl-image").animate(e,d.animationSpeed,function(){setTimeout(function(){var c=o.eq(H);j.attr("src",c.attr("href")),m.indexOf(c.attr("href"))==-1&&D.show(),a(".sl-caption").remove(),O(b),d.preloading&&T()},100)})}},V=function(){if(!G){var b=o.eq(H),c=!1;b.trigger(a.Event("close.simplelightbox")),d.history&&y(),a(".sl-image img, .sl-overlay, .sl-close, .sl-navigation, .sl-image .sl-caption, .sl-counter").fadeOut("fast",function(){d.disableScroll&&W("show"),a(".sl-wrapper, .sl-overlay").remove(),S(),c||b.trigger(a.Event("closed.simplelightbox")),c=!0}),j=a(),l=!1,G=!1}},W=function(d){var e=0;if("hide"==d){var f=b.innerWidth;if(!f){var g=c.documentElement.getBoundingClientRect();f=g.right-Math.abs(g.left)}if(c.body.clientWidth<f){var h=c.createElement("div"),i=parseInt(a("body").css("padding-right"),10);h.className="sl-scrollbar-measure",a("body").append(h),e=h.offsetWidth-h.clientWidth,a(c.body)[0].removeChild(h),a("body").data("padding",i),e>0&&a("body").addClass("hidden-scroll").css({"padding-right":i+e})}}else a("body").removeClass("hidden-scroll").css({"padding-right":a("body").data("padding")});return e};return M(),o.on("click."+A,function(b){if(L(this)){if(b.preventDefault(),G)return!1;N(a(this))}}),a(c).on("click."+A+" touchstart."+A,function(b){l&&d.docClose&&0===a(b.target).closest(".sl-image").length&&0===a(b.target).closest(".sl-navigation").length&&V()}),d.disableRightClick&&a(c).on("contextmenu",".sl-image img",function(a){return!1}),d.enableKeyboard&&a(c).on("keyup."+A,function(a){if(h=0,l){a.preventDefault();var b=a.keyCode;27==b&&V(),37!=b&&39!=a.keyCode||U(39==a.keyCode?1:-1)}}),this.open=function(b){b=b||a(this[0]),N(b)},this.next=function(){U(1)},this.prev=function(){U(-1)},this.close=function(){V()},this.destroy=function(){a(c).unbind("click."+A).unbind("keyup."+A),V(),a(".sl-overlay, .sl-wrapper").remove(),this.off("click")},this.refresh=function(){this.destroy(),a(this.selector).simpleLightbox(d)},this}}(jQuery,window,document);

/*
 Version: 1.6.0
  Author: Ken Wheeler
 Website: http://kenwheeler.github.io
    Docs: http://kenwheeler.github.io/slick
    Repo: http://github.com/kenwheeler/slick
  Issues: http://github.com/kenwheeler/slick/issues

 */
!function(a){"use strict";"function"==typeof define&&define.amd?define(["jquery"],a):"undefined"!=typeof exports?module.exports=a(require("jquery")):a(jQuery)}(function(a){"use strict";var b=window.Slick||{};b=function(){function c(c,d){var f,e=this;e.defaults={accessibility:!0,adaptiveHeight:!1,appendArrows:a(c),appendDots:a(c),arrows:!0,asNavFor:null,prevArrow:'<button type="button" data-role="none" class="slick-prev" aria-label="Previous" tabindex="0" role="button">Previous</button>',nextArrow:'<button type="button" data-role="none" class="slick-next" aria-label="Next" tabindex="0" role="button">Next</button>',autoplay:!1,autoplaySpeed:3e3,centerMode:!1,centerPadding:"50px",cssEase:"ease",customPaging:function(b,c){return a('<button type="button" data-role="none" role="button" tabindex="0" />').text(c+1)},dots:!1,dotsClass:"slick-dots",draggable:!0,easing:"linear",edgeFriction:.35,fade:!1,focusOnSelect:!1,infinite:!0,initialSlide:0,lazyLoad:"ondemand",mobileFirst:!1,pauseOnHover:!0,pauseOnFocus:!0,pauseOnDotsHover:!1,respondTo:"window",responsive:null,rows:1,rtl:!1,slide:"",slidesPerRow:1,slidesToShow:1,slidesToScroll:1,speed:500,swipe:!0,swipeToSlide:!1,touchMove:!0,touchThreshold:5,useCSS:!0,useTransform:!0,variableWidth:!1,vertical:!1,verticalSwiping:!1,waitForAnimate:!0,zIndex:1e3},e.initials={animating:!1,dragging:!1,autoPlayTimer:null,currentDirection:0,currentLeft:null,currentSlide:0,direction:1,$dots:null,listWidth:null,listHeight:null,loadIndex:0,$nextArrow:null,$prevArrow:null,slideCount:null,slideWidth:null,$slideTrack:null,$slides:null,sliding:!1,slideOffset:0,swipeLeft:null,$list:null,touchObject:{},transformsEnabled:!1,unslicked:!1},a.extend(e,e.initials),e.activeBreakpoint=null,e.animType=null,e.animProp=null,e.breakpoints=[],e.breakpointSettings=[],e.cssTransitions=!1,e.focussed=!1,e.interrupted=!1,e.hidden="hidden",e.paused=!0,e.positionProp=null,e.respondTo=null,e.rowCount=1,e.shouldClick=!0,e.$slider=a(c),e.$slidesCache=null,e.transformType=null,e.transitionType=null,e.visibilityChange="visibilitychange",e.windowWidth=0,e.windowTimer=null,f=a(c).data("slick")||{},e.options=a.extend({},e.defaults,d,f),e.currentSlide=e.options.initialSlide,e.originalSettings=e.options,"undefined"!=typeof document.mozHidden?(e.hidden="mozHidden",e.visibilityChange="mozvisibilitychange"):"undefined"!=typeof document.webkitHidden&&(e.hidden="webkitHidden",e.visibilityChange="webkitvisibilitychange"),e.autoPlay=a.proxy(e.autoPlay,e),e.autoPlayClear=a.proxy(e.autoPlayClear,e),e.autoPlayIterator=a.proxy(e.autoPlayIterator,e),e.changeSlide=a.proxy(e.changeSlide,e),e.clickHandler=a.proxy(e.clickHandler,e),e.selectHandler=a.proxy(e.selectHandler,e),e.setPosition=a.proxy(e.setPosition,e),e.swipeHandler=a.proxy(e.swipeHandler,e),e.dragHandler=a.proxy(e.dragHandler,e),e.keyHandler=a.proxy(e.keyHandler,e),e.instanceUid=b++,e.htmlExpr=/^(?:\s*(<[\w\W]+>)[^>]*)$/,e.registerBreakpoints(),e.init(!0)}var b=0;return c}(),b.prototype.activateADA=function(){var a=this;a.$slideTrack.find(".slick-active").attr({"aria-hidden":"false"}).find("a, input, button, select").attr({tabindex:"0"})},b.prototype.addSlide=b.prototype.slickAdd=function(b,c,d){var e=this;if("boolean"==typeof c)d=c,c=null;else if(0>c||c>=e.slideCount)return!1;e.unload(),"number"==typeof c?0===c&&0===e.$slides.length?a(b).appendTo(e.$slideTrack):d?a(b).insertBefore(e.$slides.eq(c)):a(b).insertAfter(e.$slides.eq(c)):d===!0?a(b).prependTo(e.$slideTrack):a(b).appendTo(e.$slideTrack),e.$slides=e.$slideTrack.children(this.options.slide),e.$slideTrack.children(this.options.slide).detach(),e.$slideTrack.append(e.$slides),e.$slides.each(function(b,c){a(c).attr("data-slick-index",b)}),e.$slidesCache=e.$slides,e.reinit()},b.prototype.animateHeight=function(){var a=this;if(1===a.options.slidesToShow&&a.options.adaptiveHeight===!0&&a.options.vertical===!1){var b=a.$slides.eq(a.currentSlide).outerHeight(!0);a.$list.animate({height:b},a.options.speed)}},b.prototype.animateSlide=function(b,c){var d={},e=this;e.animateHeight(),e.options.rtl===!0&&e.options.vertical===!1&&(b=-b),e.transformsEnabled===!1?e.options.vertical===!1?e.$slideTrack.animate({left:b},e.options.speed,e.options.easing,c):e.$slideTrack.animate({top:b},e.options.speed,e.options.easing,c):e.cssTransitions===!1?(e.options.rtl===!0&&(e.currentLeft=-e.currentLeft),a({animStart:e.currentLeft}).animate({animStart:b},{duration:e.options.speed,easing:e.options.easing,step:function(a){a=Math.ceil(a),e.options.vertical===!1?(d[e.animType]="translate("+a+"px, 0px)",e.$slideTrack.css(d)):(d[e.animType]="translate(0px,"+a+"px)",e.$slideTrack.css(d))},complete:function(){c&&c.call()}})):(e.applyTransition(),b=Math.ceil(b),e.options.vertical===!1?d[e.animType]="translate3d("+b+"px, 0px, 0px)":d[e.animType]="translate3d(0px,"+b+"px, 0px)",e.$slideTrack.css(d),c&&setTimeout(function(){e.disableTransition(),c.call()},e.options.speed))},b.prototype.getNavTarget=function(){var b=this,c=b.options.asNavFor;return c&&null!==c&&(c=a(c).not(b.$slider)),c},b.prototype.asNavFor=function(b){var c=this,d=c.getNavTarget();null!==d&&"object"==typeof d&&d.each(function(){var c=a(this).slick("getSlick");c.unslicked||c.slideHandler(b,!0)})},b.prototype.applyTransition=function(a){var b=this,c={};b.options.fade===!1?c[b.transitionType]=b.transformType+" "+b.options.speed+"ms "+b.options.cssEase:c[b.transitionType]="opacity "+b.options.speed+"ms "+b.options.cssEase,b.options.fade===!1?b.$slideTrack.css(c):b.$slides.eq(a).css(c)},b.prototype.autoPlay=function(){var a=this;a.autoPlayClear(),a.slideCount>a.options.slidesToShow&&(a.autoPlayTimer=setInterval(a.autoPlayIterator,a.options.autoplaySpeed))},b.prototype.autoPlayClear=function(){var a=this;a.autoPlayTimer&&clearInterval(a.autoPlayTimer)},b.prototype.autoPlayIterator=function(){var a=this,b=a.currentSlide+a.options.slidesToScroll;a.paused||a.interrupted||a.focussed||(a.options.infinite===!1&&(1===a.direction&&a.currentSlide+1===a.slideCount-1?a.direction=0:0===a.direction&&(b=a.currentSlide-a.options.slidesToScroll,a.currentSlide-1===0&&(a.direction=1))),a.slideHandler(b))},b.prototype.buildArrows=function(){var b=this;b.options.arrows===!0&&(b.$prevArrow=a(b.options.prevArrow).addClass("slick-arrow"),b.$nextArrow=a(b.options.nextArrow).addClass("slick-arrow"),b.slideCount>b.options.slidesToShow?(b.$prevArrow.removeClass("slick-hidden").removeAttr("aria-hidden tabindex"),b.$nextArrow.removeClass("slick-hidden").removeAttr("aria-hidden tabindex"),b.htmlExpr.test(b.options.prevArrow)&&b.$prevArrow.prependTo(b.options.appendArrows),b.htmlExpr.test(b.options.nextArrow)&&b.$nextArrow.appendTo(b.options.appendArrows),b.options.infinite!==!0&&b.$prevArrow.addClass("slick-disabled").attr("aria-disabled","true")):b.$prevArrow.add(b.$nextArrow).addClass("slick-hidden").attr({"aria-disabled":"true",tabindex:"-1"}))},b.prototype.buildDots=function(){var c,d,b=this;if(b.options.dots===!0&&b.slideCount>b.options.slidesToShow){for(b.$slider.addClass("slick-dotted"),d=a("<ul />").addClass(b.options.dotsClass),c=0;c<=b.getDotCount();c+=1)d.append(a("<li />").append(b.options.customPaging.call(this,b,c)));b.$dots=d.appendTo(b.options.appendDots),b.$dots.find("li").first().addClass("slick-active").attr("aria-hidden","false")}},b.prototype.buildOut=function(){var b=this;b.$slides=b.$slider.children(b.options.slide+":not(.slick-cloned)").addClass("slick-slide"),b.slideCount=b.$slides.length,b.$slides.each(function(b,c){a(c).attr("data-slick-index",b).data("originalStyling",a(c).attr("style")||"")}),b.$slider.addClass("slick-slider"),b.$slideTrack=0===b.slideCount?a('<div class="slick-track"/>').appendTo(b.$slider):b.$slides.wrapAll('<div class="slick-track"/>').parent(),b.$list=b.$slideTrack.wrap('<div aria-live="polite" class="slick-list"/>').parent(),b.$slideTrack.css("opacity",0),(b.options.centerMode===!0||b.options.swipeToSlide===!0)&&(b.options.slidesToScroll=1),a("img[data-lazy]",b.$slider).not("[src]").addClass("slick-loading"),b.setupInfinite(),b.buildArrows(),b.buildDots(),b.updateDots(),b.setSlideClasses("number"==typeof b.currentSlide?b.currentSlide:0),b.options.draggable===!0&&b.$list.addClass("draggable")},b.prototype.buildRows=function(){var b,c,d,e,f,g,h,a=this;if(e=document.createDocumentFragment(),g=a.$slider.children(),a.options.rows>1){for(h=a.options.slidesPerRow*a.options.rows,f=Math.ceil(g.length/h),b=0;f>b;b++){var i=document.createElement("div");for(c=0;c<a.options.rows;c++){var j=document.createElement("div");for(d=0;d<a.options.slidesPerRow;d++){var k=b*h+(c*a.options.slidesPerRow+d);g.get(k)&&j.appendChild(g.get(k))}i.appendChild(j)}e.appendChild(i)}a.$slider.empty().append(e),a.$slider.children().children().children().css({width:100/a.options.slidesPerRow+"%",display:"inline-block"})}},b.prototype.checkResponsive=function(b,c){var e,f,g,d=this,h=!1,i=d.$slider.width(),j=window.innerWidth||a(window).width();if("window"===d.respondTo?g=j:"slider"===d.respondTo?g=i:"min"===d.respondTo&&(g=Math.min(j,i)),d.options.responsive&&d.options.responsive.length&&null!==d.options.responsive){f=null;for(e in d.breakpoints)d.breakpoints.hasOwnProperty(e)&&(d.originalSettings.mobileFirst===!1?g<d.breakpoints[e]&&(f=d.breakpoints[e]):g>d.breakpoints[e]&&(f=d.breakpoints[e]));null!==f?null!==d.activeBreakpoint?(f!==d.activeBreakpoint||c)&&(d.activeBreakpoint=f,"unslick"===d.breakpointSettings[f]?d.unslick(f):(d.options=a.extend({},d.originalSettings,d.breakpointSettings[f]),b===!0&&(d.currentSlide=d.options.initialSlide),d.refresh(b)),h=f):(d.activeBreakpoint=f,"unslick"===d.breakpointSettings[f]?d.unslick(f):(d.options=a.extend({},d.originalSettings,d.breakpointSettings[f]),b===!0&&(d.currentSlide=d.options.initialSlide),d.refresh(b)),h=f):null!==d.activeBreakpoint&&(d.activeBreakpoint=null,d.options=d.originalSettings,b===!0&&(d.currentSlide=d.options.initialSlide),d.refresh(b),h=f),b||h===!1||d.$slider.trigger("breakpoint",[d,h])}},b.prototype.changeSlide=function(b,c){var f,g,h,d=this,e=a(b.currentTarget);switch(e.is("a")&&b.preventDefault(),e.is("li")||(e=e.closest("li")),h=d.slideCount%d.options.slidesToScroll!==0,f=h?0:(d.slideCount-d.currentSlide)%d.options.slidesToScroll,b.data.message){case"previous":g=0===f?d.options.slidesToScroll:d.options.slidesToShow-f,d.slideCount>d.options.slidesToShow&&d.slideHandler(d.currentSlide-g,!1,c);break;case"next":g=0===f?d.options.slidesToScroll:f,d.slideCount>d.options.slidesToShow&&d.slideHandler(d.currentSlide+g,!1,c);break;case"index":var i=0===b.data.index?0:b.data.index||e.index()*d.options.slidesToScroll;d.slideHandler(d.checkNavigable(i),!1,c),e.children().trigger("focus");break;default:return}},b.prototype.checkNavigable=function(a){var c,d,b=this;if(c=b.getNavigableIndexes(),d=0,a>c[c.length-1])a=c[c.length-1];else for(var e in c){if(a<c[e]){a=d;break}d=c[e]}return a},b.prototype.cleanUpEvents=function(){var b=this;b.options.dots&&null!==b.$dots&&a("li",b.$dots).off("click.slick",b.changeSlide).off("mouseenter.slick",a.proxy(b.interrupt,b,!0)).off("mouseleave.slick",a.proxy(b.interrupt,b,!1)),b.$slider.off("focus.slick blur.slick"),b.options.arrows===!0&&b.slideCount>b.options.slidesToShow&&(b.$prevArrow&&b.$prevArrow.off("click.slick",b.changeSlide),b.$nextArrow&&b.$nextArrow.off("click.slick",b.changeSlide)),b.$list.off("touchstart.slick mousedown.slick",b.swipeHandler),b.$list.off("touchmove.slick mousemove.slick",b.swipeHandler),b.$list.off("touchend.slick mouseup.slick",b.swipeHandler),b.$list.off("touchcancel.slick mouseleave.slick",b.swipeHandler),b.$list.off("click.slick",b.clickHandler),a(document).off(b.visibilityChange,b.visibility),b.cleanUpSlideEvents(),b.options.accessibility===!0&&b.$list.off("keydown.slick",b.keyHandler),b.options.focusOnSelect===!0&&a(b.$slideTrack).children().off("click.slick",b.selectHandler),a(window).off("orientationchange.slick.slick-"+b.instanceUid,b.orientationChange),a(window).off("resize.slick.slick-"+b.instanceUid,b.resize),a("[draggable!=true]",b.$slideTrack).off("dragstart",b.preventDefault),a(window).off("load.slick.slick-"+b.instanceUid,b.setPosition),a(document).off("ready.slick.slick-"+b.instanceUid,b.setPosition)},b.prototype.cleanUpSlideEvents=function(){var b=this;b.$list.off("mouseenter.slick",a.proxy(b.interrupt,b,!0)),b.$list.off("mouseleave.slick",a.proxy(b.interrupt,b,!1))},b.prototype.cleanUpRows=function(){var b,a=this;a.options.rows>1&&(b=a.$slides.children().children(),b.removeAttr("style"),a.$slider.empty().append(b))},b.prototype.clickHandler=function(a){var b=this;b.shouldClick===!1&&(a.stopImmediatePropagation(),a.stopPropagation(),a.preventDefault())},b.prototype.destroy=function(b){var c=this;c.autoPlayClear(),c.touchObject={},c.cleanUpEvents(),a(".slick-cloned",c.$slider).detach(),c.$dots&&c.$dots.remove(),c.$prevArrow&&c.$prevArrow.length&&(c.$prevArrow.removeClass("slick-disabled slick-arrow slick-hidden").removeAttr("aria-hidden aria-disabled tabindex").css("display",""),c.htmlExpr.test(c.options.prevArrow)&&c.$prevArrow.remove()),c.$nextArrow&&c.$nextArrow.length&&(c.$nextArrow.removeClass("slick-disabled slick-arrow slick-hidden").removeAttr("aria-hidden aria-disabled tabindex").css("display",""),c.htmlExpr.test(c.options.nextArrow)&&c.$nextArrow.remove()),c.$slides&&(c.$slides.removeClass("slick-slide slick-active slick-center slick-visible slick-current").removeAttr("aria-hidden").removeAttr("data-slick-index").each(function(){a(this).attr("style",a(this).data("originalStyling"))}),c.$slideTrack.children(this.options.slide).detach(),c.$slideTrack.detach(),c.$list.detach(),c.$slider.append(c.$slides)),c.cleanUpRows(),c.$slider.removeClass("slick-slider"),c.$slider.removeClass("slick-initialized"),c.$slider.removeClass("slick-dotted"),c.unslicked=!0,b||c.$slider.trigger("destroy",[c])},b.prototype.disableTransition=function(a){var b=this,c={};c[b.transitionType]="",b.options.fade===!1?b.$slideTrack.css(c):b.$slides.eq(a).css(c)},b.prototype.fadeSlide=function(a,b){var c=this;c.cssTransitions===!1?(c.$slides.eq(a).css({zIndex:c.options.zIndex}),c.$slides.eq(a).animate({opacity:1},c.options.speed,c.options.easing,b)):(c.applyTransition(a),c.$slides.eq(a).css({opacity:1,zIndex:c.options.zIndex}),b&&setTimeout(function(){c.disableTransition(a),b.call()},c.options.speed))},b.prototype.fadeSlideOut=function(a){var b=this;b.cssTransitions===!1?b.$slides.eq(a).animate({opacity:0,zIndex:b.options.zIndex-2},b.options.speed,b.options.easing):(b.applyTransition(a),b.$slides.eq(a).css({opacity:0,zIndex:b.options.zIndex-2}))},b.prototype.filterSlides=b.prototype.slickFilter=function(a){var b=this;null!==a&&(b.$slidesCache=b.$slides,b.unload(),b.$slideTrack.children(this.options.slide).detach(),b.$slidesCache.filter(a).appendTo(b.$slideTrack),b.reinit())},b.prototype.focusHandler=function(){var b=this;b.$slider.off("focus.slick blur.slick").on("focus.slick blur.slick","*:not(.slick-arrow)",function(c){c.stopImmediatePropagation();var d=a(this);setTimeout(function(){b.options.pauseOnFocus&&(b.focussed=d.is(":focus"),b.autoPlay())},0)})},b.prototype.getCurrent=b.prototype.slickCurrentSlide=function(){var a=this;return a.currentSlide},b.prototype.getDotCount=function(){var a=this,b=0,c=0,d=0;if(a.options.infinite===!0)for(;b<a.slideCount;)++d,b=c+a.options.slidesToScroll,c+=a.options.slidesToScroll<=a.options.slidesToShow?a.options.slidesToScroll:a.options.slidesToShow;else if(a.options.centerMode===!0)d=a.slideCount;else if(a.options.asNavFor)for(;b<a.slideCount;)++d,b=c+a.options.slidesToScroll,c+=a.options.slidesToScroll<=a.options.slidesToShow?a.options.slidesToScroll:a.options.slidesToShow;else d=1+Math.ceil((a.slideCount-a.options.slidesToShow)/a.options.slidesToScroll);return d-1},b.prototype.getLeft=function(a){var c,d,f,b=this,e=0;return b.slideOffset=0,d=b.$slides.first().outerHeight(!0),b.options.infinite===!0?(b.slideCount>b.options.slidesToShow&&(b.slideOffset=b.slideWidth*b.options.slidesToShow*-1,e=d*b.options.slidesToShow*-1),b.slideCount%b.options.slidesToScroll!==0&&a+b.options.slidesToScroll>b.slideCount&&b.slideCount>b.options.slidesToShow&&(a>b.slideCount?(b.slideOffset=(b.options.slidesToShow-(a-b.slideCount))*b.slideWidth*-1,e=(b.options.slidesToShow-(a-b.slideCount))*d*-1):(b.slideOffset=b.slideCount%b.options.slidesToScroll*b.slideWidth*-1,e=b.slideCount%b.options.slidesToScroll*d*-1))):a+b.options.slidesToShow>b.slideCount&&(b.slideOffset=(a+b.options.slidesToShow-b.slideCount)*b.slideWidth,e=(a+b.options.slidesToShow-b.slideCount)*d),b.slideCount<=b.options.slidesToShow&&(b.slideOffset=0,e=0),b.options.centerMode===!0&&b.options.infinite===!0?b.slideOffset+=b.slideWidth*Math.floor(b.options.slidesToShow/2)-b.slideWidth:b.options.centerMode===!0&&(b.slideOffset=0,b.slideOffset+=b.slideWidth*Math.floor(b.options.slidesToShow/2)),c=b.options.vertical===!1?a*b.slideWidth*-1+b.slideOffset:a*d*-1+e,b.options.variableWidth===!0&&(f=b.slideCount<=b.options.slidesToShow||b.options.infinite===!1?b.$slideTrack.children(".slick-slide").eq(a):b.$slideTrack.children(".slick-slide").eq(a+b.options.slidesToShow),c=b.options.rtl===!0?f[0]?-1*(b.$slideTrack.width()-f[0].offsetLeft-f.width()):0:f[0]?-1*f[0].offsetLeft:0,b.options.centerMode===!0&&(f=b.slideCount<=b.options.slidesToShow||b.options.infinite===!1?b.$slideTrack.children(".slick-slide").eq(a):b.$slideTrack.children(".slick-slide").eq(a+b.options.slidesToShow+1),c=b.options.rtl===!0?f[0]?-1*(b.$slideTrack.width()-f[0].offsetLeft-f.width()):0:f[0]?-1*f[0].offsetLeft:0,c+=(b.$list.width()-f.outerWidth())/2)),c},b.prototype.getOption=b.prototype.slickGetOption=function(a){var b=this;return b.options[a]},b.prototype.getNavigableIndexes=function(){var e,a=this,b=0,c=0,d=[];for(a.options.infinite===!1?e=a.slideCount:(b=-1*a.options.slidesToScroll,c=-1*a.options.slidesToScroll,e=2*a.slideCount);e>b;)d.push(b),b=c+a.options.slidesToScroll,c+=a.options.slidesToScroll<=a.options.slidesToShow?a.options.slidesToScroll:a.options.slidesToShow;return d},b.prototype.getSlick=function(){return this},b.prototype.getSlideCount=function(){var c,d,e,b=this;return e=b.options.centerMode===!0?b.slideWidth*Math.floor(b.options.slidesToShow/2):0,b.options.swipeToSlide===!0?(b.$slideTrack.find(".slick-slide").each(function(c,f){return f.offsetLeft-e+a(f).outerWidth()/2>-1*b.swipeLeft?(d=f,!1):void 0}),c=Math.abs(a(d).attr("data-slick-index")-b.currentSlide)||1):b.options.slidesToScroll},b.prototype.goTo=b.prototype.slickGoTo=function(a,b){var c=this;c.changeSlide({data:{message:"index",index:parseInt(a)}},b)},b.prototype.init=function(b){var c=this;a(c.$slider).hasClass("slick-initialized")||(a(c.$slider).addClass("slick-initialized"),c.buildRows(),c.buildOut(),c.setProps(),c.startLoad(),c.loadSlider(),c.initializeEvents(),c.updateArrows(),c.updateDots(),c.checkResponsive(!0),c.focusHandler()),b&&c.$slider.trigger("init",[c]),c.options.accessibility===!0&&c.initADA(),c.options.autoplay&&(c.paused=!1,c.autoPlay())},b.prototype.initADA=function(){var b=this;b.$slides.add(b.$slideTrack.find(".slick-cloned")).attr({"aria-hidden":"true",tabindex:"-1"}).find("a, input, button, select").attr({tabindex:"-1"}),b.$slideTrack.attr("role","listbox"),b.$slides.not(b.$slideTrack.find(".slick-cloned")).each(function(c){a(this).attr({role:"option","aria-describedby":"slick-slide"+b.instanceUid+c})}),null!==b.$dots&&b.$dots.attr("role","tablist").find("li").each(function(c){a(this).attr({role:"presentation","aria-selected":"false","aria-controls":"navigation"+b.instanceUid+c,id:"slick-slide"+b.instanceUid+c})}).first().attr("aria-selected","true").end().find("button").attr("role","button").end().closest("div").attr("role","toolbar"),b.activateADA()},b.prototype.initArrowEvents=function(){var a=this;a.options.arrows===!0&&a.slideCount>a.options.slidesToShow&&(a.$prevArrow.off("click.slick").on("click.slick",{message:"previous"},a.changeSlide),a.$nextArrow.off("click.slick").on("click.slick",{message:"next"},a.changeSlide))},b.prototype.initDotEvents=function(){var b=this;b.options.dots===!0&&b.slideCount>b.options.slidesToShow&&a("li",b.$dots).on("click.slick",{message:"index"},b.changeSlide),b.options.dots===!0&&b.options.pauseOnDotsHover===!0&&a("li",b.$dots).on("mouseenter.slick",a.proxy(b.interrupt,b,!0)).on("mouseleave.slick",a.proxy(b.interrupt,b,!1))},b.prototype.initSlideEvents=function(){var b=this;b.options.pauseOnHover&&(b.$list.on("mouseenter.slick",a.proxy(b.interrupt,b,!0)),b.$list.on("mouseleave.slick",a.proxy(b.interrupt,b,!1)))},b.prototype.initializeEvents=function(){var b=this;b.initArrowEvents(),b.initDotEvents(),b.initSlideEvents(),b.$list.on("touchstart.slick mousedown.slick",{action:"start"},b.swipeHandler),b.$list.on("touchmove.slick mousemove.slick",{action:"move"},b.swipeHandler),b.$list.on("touchend.slick mouseup.slick",{action:"end"},b.swipeHandler),b.$list.on("touchcancel.slick mouseleave.slick",{action:"end"},b.swipeHandler),b.$list.on("click.slick",b.clickHandler),a(document).on(b.visibilityChange,a.proxy(b.visibility,b)),b.options.accessibility===!0&&b.$list.on("keydown.slick",b.keyHandler),b.options.focusOnSelect===!0&&a(b.$slideTrack).children().on("click.slick",b.selectHandler),a(window).on("orientationchange.slick.slick-"+b.instanceUid,a.proxy(b.orientationChange,b)),a(window).on("resize.slick.slick-"+b.instanceUid,a.proxy(b.resize,b)),a("[draggable!=true]",b.$slideTrack).on("dragstart",b.preventDefault),a(window).on("load.slick.slick-"+b.instanceUid,b.setPosition),a(document).on("ready.slick.slick-"+b.instanceUid,b.setPosition)},b.prototype.initUI=function(){var a=this;a.options.arrows===!0&&a.slideCount>a.options.slidesToShow&&(a.$prevArrow.show(),a.$nextArrow.show()),a.options.dots===!0&&a.slideCount>a.options.slidesToShow&&a.$dots.show()},b.prototype.keyHandler=function(a){var b=this;a.target.tagName.match("TEXTAREA|INPUT|SELECT")||(37===a.keyCode&&b.options.accessibility===!0?b.changeSlide({data:{message:b.options.rtl===!0?"next":"previous"}}):39===a.keyCode&&b.options.accessibility===!0&&b.changeSlide({data:{message:b.options.rtl===!0?"previous":"next"}}))},b.prototype.lazyLoad=function(){function g(c){a("img[data-lazy]",c).each(function(){var c=a(this),d=a(this).attr("data-lazy"),e=document.createElement("img");e.onload=function(){c.animate({opacity:0},100,function(){c.attr("src",d).animate({opacity:1},200,function(){c.removeAttr("data-lazy").removeClass("slick-loading")}),b.$slider.trigger("lazyLoaded",[b,c,d])})},e.onerror=function(){c.removeAttr("data-lazy").removeClass("slick-loading").addClass("slick-lazyload-error"),b.$slider.trigger("lazyLoadError",[b,c,d])},e.src=d})}var c,d,e,f,b=this;b.options.centerMode===!0?b.options.infinite===!0?(e=b.currentSlide+(b.options.slidesToShow/2+1),f=e+b.options.slidesToShow+2):(e=Math.max(0,b.currentSlide-(b.options.slidesToShow/2+1)),f=2+(b.options.slidesToShow/2+1)+b.currentSlide):(e=b.options.infinite?b.options.slidesToShow+b.currentSlide:b.currentSlide,f=Math.ceil(e+b.options.slidesToShow),b.options.fade===!0&&(e>0&&e--,f<=b.slideCount&&f++)),c=b.$slider.find(".slick-slide").slice(e,f),g(c),b.slideCount<=b.options.slidesToShow?(d=b.$slider.find(".slick-slide"),g(d)):b.currentSlide>=b.slideCount-b.options.slidesToShow?(d=b.$slider.find(".slick-cloned").slice(0,b.options.slidesToShow),g(d)):0===b.currentSlide&&(d=b.$slider.find(".slick-cloned").slice(-1*b.options.slidesToShow),g(d))},b.prototype.loadSlider=function(){var a=this;a.setPosition(),a.$slideTrack.css({opacity:1}),a.$slider.removeClass("slick-loading"),a.initUI(),"progressive"===a.options.lazyLoad&&a.progressiveLazyLoad()},b.prototype.next=b.prototype.slickNext=function(){var a=this;a.changeSlide({data:{message:"next"}})},b.prototype.orientationChange=function(){var a=this;a.checkResponsive(),a.setPosition()},b.prototype.pause=b.prototype.slickPause=function(){var a=this;a.autoPlayClear(),a.paused=!0},b.prototype.play=b.prototype.slickPlay=function(){var a=this;a.autoPlay(),a.options.autoplay=!0,a.paused=!1,a.focussed=!1,a.interrupted=!1},b.prototype.postSlide=function(a){var b=this;b.unslicked||(b.$slider.trigger("afterChange",[b,a]),b.animating=!1,b.setPosition(),b.swipeLeft=null,b.options.autoplay&&b.autoPlay(),b.options.accessibility===!0&&b.initADA())},b.prototype.prev=b.prototype.slickPrev=function(){var a=this;a.changeSlide({data:{message:"previous"}})},b.prototype.preventDefault=function(a){a.preventDefault()},b.prototype.progressiveLazyLoad=function(b){b=b||1;var e,f,g,c=this,d=a("img[data-lazy]",c.$slider);d.length?(e=d.first(),f=e.attr("data-lazy"),g=document.createElement("img"),g.onload=function(){e.attr("src",f).removeAttr("data-lazy").removeClass("slick-loading"),c.options.adaptiveHeight===!0&&c.setPosition(),c.$slider.trigger("lazyLoaded",[c,e,f]),c.progressiveLazyLoad()},g.onerror=function(){3>b?setTimeout(function(){c.progressiveLazyLoad(b+1)},500):(e.removeAttr("data-lazy").removeClass("slick-loading").addClass("slick-lazyload-error"),c.$slider.trigger("lazyLoadError",[c,e,f]),c.progressiveLazyLoad())},g.src=f):c.$slider.trigger("allImagesLoaded",[c])},b.prototype.refresh=function(b){var d,e,c=this;e=c.slideCount-c.options.slidesToShow,!c.options.infinite&&c.currentSlide>e&&(c.currentSlide=e),c.slideCount<=c.options.slidesToShow&&(c.currentSlide=0),d=c.currentSlide,c.destroy(!0),a.extend(c,c.initials,{currentSlide:d}),c.init(),b||c.changeSlide({data:{message:"index",index:d}},!1)},b.prototype.registerBreakpoints=function(){var c,d,e,b=this,f=b.options.responsive||null;if("array"===a.type(f)&&f.length){b.respondTo=b.options.respondTo||"window";for(c in f)if(e=b.breakpoints.length-1,d=f[c].breakpoint,f.hasOwnProperty(c)){for(;e>=0;)b.breakpoints[e]&&b.breakpoints[e]===d&&b.breakpoints.splice(e,1),e--;b.breakpoints.push(d),b.breakpointSettings[d]=f[c].settings}b.breakpoints.sort(function(a,c){return b.options.mobileFirst?a-c:c-a})}},b.prototype.reinit=function(){var b=this;b.$slides=b.$slideTrack.children(b.options.slide).addClass("slick-slide"),b.slideCount=b.$slides.length,b.currentSlide>=b.slideCount&&0!==b.currentSlide&&(b.currentSlide=b.currentSlide-b.options.slidesToScroll),b.slideCount<=b.options.slidesToShow&&(b.currentSlide=0),b.registerBreakpoints(),b.setProps(),b.setupInfinite(),b.buildArrows(),b.updateArrows(),b.initArrowEvents(),b.buildDots(),b.updateDots(),b.initDotEvents(),b.cleanUpSlideEvents(),b.initSlideEvents(),b.checkResponsive(!1,!0),b.options.focusOnSelect===!0&&a(b.$slideTrack).children().on("click.slick",b.selectHandler),b.setSlideClasses("number"==typeof b.currentSlide?b.currentSlide:0),b.setPosition(),b.focusHandler(),b.paused=!b.options.autoplay,b.autoPlay(),b.$slider.trigger("reInit",[b])},b.prototype.resize=function(){var b=this;a(window).width()!==b.windowWidth&&(clearTimeout(b.windowDelay),b.windowDelay=window.setTimeout(function(){b.windowWidth=a(window).width(),b.checkResponsive(),b.unslicked||b.setPosition()},50))},b.prototype.removeSlide=b.prototype.slickRemove=function(a,b,c){var d=this;return"boolean"==typeof a?(b=a,a=b===!0?0:d.slideCount-1):a=b===!0?--a:a,d.slideCount<1||0>a||a>d.slideCount-1?!1:(d.unload(),c===!0?d.$slideTrack.children().remove():d.$slideTrack.children(this.options.slide).eq(a).remove(),d.$slides=d.$slideTrack.children(this.options.slide),d.$slideTrack.children(this.options.slide).detach(),d.$slideTrack.append(d.$slides),d.$slidesCache=d.$slides,void d.reinit())},b.prototype.setCSS=function(a){var d,e,b=this,c={};b.options.rtl===!0&&(a=-a),d="left"==b.positionProp?Math.ceil(a)+"px":"0px",e="top"==b.positionProp?Math.ceil(a)+"px":"0px",c[b.positionProp]=a,b.transformsEnabled===!1?b.$slideTrack.css(c):(c={},b.cssTransitions===!1?(c[b.animType]="translate("+d+", "+e+")",b.$slideTrack.css(c)):(c[b.animType]="translate3d("+d+", "+e+", 0px)",b.$slideTrack.css(c)))},b.prototype.setDimensions=function(){var a=this;a.options.vertical===!1?a.options.centerMode===!0&&a.$list.css({padding:"0px "+a.options.centerPadding}):(a.$list.height(a.$slides.first().outerHeight(!0)*a.options.slidesToShow),a.options.centerMode===!0&&a.$list.css({padding:a.options.centerPadding+" 0px"})),a.listWidth=a.$list.width(),a.listHeight=a.$list.height(),a.options.vertical===!1&&a.options.variableWidth===!1?(a.slideWidth=Math.ceil(a.listWidth/a.options.slidesToShow),a.$slideTrack.width(Math.ceil(a.slideWidth*a.$slideTrack.children(".slick-slide").length))):a.options.variableWidth===!0?a.$slideTrack.width(5e3*a.slideCount):(a.slideWidth=Math.ceil(a.listWidth),a.$slideTrack.height(Math.ceil(a.$slides.first().outerHeight(!0)*a.$slideTrack.children(".slick-slide").length)));var b=a.$slides.first().outerWidth(!0)-a.$slides.first().width();a.options.variableWidth===!1&&a.$slideTrack.children(".slick-slide").width(a.slideWidth-b)},b.prototype.setFade=function(){var c,b=this;b.$slides.each(function(d,e){c=b.slideWidth*d*-1,b.options.rtl===!0?a(e).css({position:"relative",right:c,top:0,zIndex:b.options.zIndex-2,opacity:0}):a(e).css({position:"relative",left:c,top:0,zIndex:b.options.zIndex-2,opacity:0})}),b.$slides.eq(b.currentSlide).css({zIndex:b.options.zIndex-1,opacity:1})},b.prototype.setHeight=function(){var a=this;if(1===a.options.slidesToShow&&a.options.adaptiveHeight===!0&&a.options.vertical===!1){var b=a.$slides.eq(a.currentSlide).outerHeight(!0);a.$list.css("height",b)}},b.prototype.setOption=b.prototype.slickSetOption=function(){var c,d,e,f,h,b=this,g=!1;if("object"===a.type(arguments[0])?(e=arguments[0],g=arguments[1],h="multiple"):"string"===a.type(arguments[0])&&(e=arguments[0],f=arguments[1],g=arguments[2],"responsive"===arguments[0]&&"array"===a.type(arguments[1])?h="responsive":"undefined"!=typeof arguments[1]&&(h="single")),"single"===h)b.options[e]=f;else if("multiple"===h)a.each(e,function(a,c){b.options[a]=c});else if("responsive"===h)for(d in f)if("array"!==a.type(b.options.responsive))b.options.responsive=[f[d]];else{for(c=b.options.responsive.length-1;c>=0;)b.options.responsive[c].breakpoint===f[d].breakpoint&&b.options.responsive.splice(c,1),c--;b.options.responsive.push(f[d])}g&&(b.unload(),b.reinit())},b.prototype.setPosition=function(){var a=this;a.setDimensions(),a.setHeight(),a.options.fade===!1?a.setCSS(a.getLeft(a.currentSlide)):a.setFade(),a.$slider.trigger("setPosition",[a])},b.prototype.setProps=function(){var a=this,b=document.body.style;a.positionProp=a.options.vertical===!0?"top":"left","top"===a.positionProp?a.$slider.addClass("slick-vertical"):a.$slider.removeClass("slick-vertical"),(void 0!==b.WebkitTransition||void 0!==b.MozTransition||void 0!==b.msTransition)&&a.options.useCSS===!0&&(a.cssTransitions=!0),a.options.fade&&("number"==typeof a.options.zIndex?a.options.zIndex<3&&(a.options.zIndex=3):a.options.zIndex=a.defaults.zIndex),void 0!==b.OTransform&&(a.animType="OTransform",a.transformType="-o-transform",a.transitionType="OTransition",void 0===b.perspectiveProperty&&void 0===b.webkitPerspective&&(a.animType=!1)),void 0!==b.MozTransform&&(a.animType="MozTransform",a.transformType="-moz-transform",a.transitionType="MozTransition",void 0===b.perspectiveProperty&&void 0===b.MozPerspective&&(a.animType=!1)),void 0!==b.webkitTransform&&(a.animType="webkitTransform",a.transformType="-webkit-transform",a.transitionType="webkitTransition",void 0===b.perspectiveProperty&&void 0===b.webkitPerspective&&(a.animType=!1)),void 0!==b.msTransform&&(a.animType="msTransform",a.transformType="-ms-transform",a.transitionType="msTransition",void 0===b.msTransform&&(a.animType=!1)),void 0!==b.transform&&a.animType!==!1&&(a.animType="transform",a.transformType="transform",a.transitionType="transition"),a.transformsEnabled=a.options.useTransform&&null!==a.animType&&a.animType!==!1},b.prototype.setSlideClasses=function(a){var c,d,e,f,b=this;d=b.$slider.find(".slick-slide").removeClass("slick-active slick-center slick-current").attr("aria-hidden","true"),b.$slides.eq(a).addClass("slick-current"),b.options.centerMode===!0?(c=Math.floor(b.options.slidesToShow/2),b.options.infinite===!0&&(a>=c&&a<=b.slideCount-1-c?b.$slides.slice(a-c,a+c+1).addClass("slick-active").attr("aria-hidden","false"):(e=b.options.slidesToShow+a,
d.slice(e-c+1,e+c+2).addClass("slick-active").attr("aria-hidden","false")),0===a?d.eq(d.length-1-b.options.slidesToShow).addClass("slick-center"):a===b.slideCount-1&&d.eq(b.options.slidesToShow).addClass("slick-center")),b.$slides.eq(a).addClass("slick-center")):a>=0&&a<=b.slideCount-b.options.slidesToShow?b.$slides.slice(a,a+b.options.slidesToShow).addClass("slick-active").attr("aria-hidden","false"):d.length<=b.options.slidesToShow?d.addClass("slick-active").attr("aria-hidden","false"):(f=b.slideCount%b.options.slidesToShow,e=b.options.infinite===!0?b.options.slidesToShow+a:a,b.options.slidesToShow==b.options.slidesToScroll&&b.slideCount-a<b.options.slidesToShow?d.slice(e-(b.options.slidesToShow-f),e+f).addClass("slick-active").attr("aria-hidden","false"):d.slice(e,e+b.options.slidesToShow).addClass("slick-active").attr("aria-hidden","false")),"ondemand"===b.options.lazyLoad&&b.lazyLoad()},b.prototype.setupInfinite=function(){var c,d,e,b=this;if(b.options.fade===!0&&(b.options.centerMode=!1),b.options.infinite===!0&&b.options.fade===!1&&(d=null,b.slideCount>b.options.slidesToShow)){for(e=b.options.centerMode===!0?b.options.slidesToShow+1:b.options.slidesToShow,c=b.slideCount;c>b.slideCount-e;c-=1)d=c-1,a(b.$slides[d]).clone(!0).attr("id","").attr("data-slick-index",d-b.slideCount).prependTo(b.$slideTrack).addClass("slick-cloned");for(c=0;e>c;c+=1)d=c,a(b.$slides[d]).clone(!0).attr("id","").attr("data-slick-index",d+b.slideCount).appendTo(b.$slideTrack).addClass("slick-cloned");b.$slideTrack.find(".slick-cloned").find("[id]").each(function(){a(this).attr("id","")})}},b.prototype.interrupt=function(a){var b=this;a||b.autoPlay(),b.interrupted=a},b.prototype.selectHandler=function(b){var c=this,d=a(b.target).is(".slick-slide")?a(b.target):a(b.target).parents(".slick-slide"),e=parseInt(d.attr("data-slick-index"));return e||(e=0),c.slideCount<=c.options.slidesToShow?(c.setSlideClasses(e),void c.asNavFor(e)):void c.slideHandler(e)},b.prototype.slideHandler=function(a,b,c){var d,e,f,g,j,h=null,i=this;return b=b||!1,i.animating===!0&&i.options.waitForAnimate===!0||i.options.fade===!0&&i.currentSlide===a||i.slideCount<=i.options.slidesToShow?void 0:(b===!1&&i.asNavFor(a),d=a,h=i.getLeft(d),g=i.getLeft(i.currentSlide),i.currentLeft=null===i.swipeLeft?g:i.swipeLeft,i.options.infinite===!1&&i.options.centerMode===!1&&(0>a||a>i.getDotCount()*i.options.slidesToScroll)?void(i.options.fade===!1&&(d=i.currentSlide,c!==!0?i.animateSlide(g,function(){i.postSlide(d)}):i.postSlide(d))):i.options.infinite===!1&&i.options.centerMode===!0&&(0>a||a>i.slideCount-i.options.slidesToScroll)?void(i.options.fade===!1&&(d=i.currentSlide,c!==!0?i.animateSlide(g,function(){i.postSlide(d)}):i.postSlide(d))):(i.options.autoplay&&clearInterval(i.autoPlayTimer),e=0>d?i.slideCount%i.options.slidesToScroll!==0?i.slideCount-i.slideCount%i.options.slidesToScroll:i.slideCount+d:d>=i.slideCount?i.slideCount%i.options.slidesToScroll!==0?0:d-i.slideCount:d,i.animating=!0,i.$slider.trigger("beforeChange",[i,i.currentSlide,e]),f=i.currentSlide,i.currentSlide=e,i.setSlideClasses(i.currentSlide),i.options.asNavFor&&(j=i.getNavTarget(),j=j.slick("getSlick"),j.slideCount<=j.options.slidesToShow&&j.setSlideClasses(i.currentSlide)),i.updateDots(),i.updateArrows(),i.options.fade===!0?(c!==!0?(i.fadeSlideOut(f),i.fadeSlide(e,function(){i.postSlide(e)})):i.postSlide(e),void i.animateHeight()):void(c!==!0?i.animateSlide(h,function(){i.postSlide(e)}):i.postSlide(e))))},b.prototype.startLoad=function(){var a=this;a.options.arrows===!0&&a.slideCount>a.options.slidesToShow&&(a.$prevArrow.hide(),a.$nextArrow.hide()),a.options.dots===!0&&a.slideCount>a.options.slidesToShow&&a.$dots.hide(),a.$slider.addClass("slick-loading")},b.prototype.swipeDirection=function(){var a,b,c,d,e=this;return a=e.touchObject.startX-e.touchObject.curX,b=e.touchObject.startY-e.touchObject.curY,c=Math.atan2(b,a),d=Math.round(180*c/Math.PI),0>d&&(d=360-Math.abs(d)),45>=d&&d>=0?e.options.rtl===!1?"left":"right":360>=d&&d>=315?e.options.rtl===!1?"left":"right":d>=135&&225>=d?e.options.rtl===!1?"right":"left":e.options.verticalSwiping===!0?d>=35&&135>=d?"down":"up":"vertical"},b.prototype.swipeEnd=function(a){var c,d,b=this;if(b.dragging=!1,b.interrupted=!1,b.shouldClick=b.touchObject.swipeLength>10?!1:!0,void 0===b.touchObject.curX)return!1;if(b.touchObject.edgeHit===!0&&b.$slider.trigger("edge",[b,b.swipeDirection()]),b.touchObject.swipeLength>=b.touchObject.minSwipe){switch(d=b.swipeDirection()){case"left":case"down":c=b.options.swipeToSlide?b.checkNavigable(b.currentSlide+b.getSlideCount()):b.currentSlide+b.getSlideCount(),b.currentDirection=0;break;case"right":case"up":c=b.options.swipeToSlide?b.checkNavigable(b.currentSlide-b.getSlideCount()):b.currentSlide-b.getSlideCount(),b.currentDirection=1}"vertical"!=d&&(b.slideHandler(c),b.touchObject={},b.$slider.trigger("swipe",[b,d]))}else b.touchObject.startX!==b.touchObject.curX&&(b.slideHandler(b.currentSlide),b.touchObject={})},b.prototype.swipeHandler=function(a){var b=this;if(!(b.options.swipe===!1||"ontouchend"in document&&b.options.swipe===!1||b.options.draggable===!1&&-1!==a.type.indexOf("mouse")))switch(b.touchObject.fingerCount=a.originalEvent&&void 0!==a.originalEvent.touches?a.originalEvent.touches.length:1,b.touchObject.minSwipe=b.listWidth/b.options.touchThreshold,b.options.verticalSwiping===!0&&(b.touchObject.minSwipe=b.listHeight/b.options.touchThreshold),a.data.action){case"start":b.swipeStart(a);break;case"move":b.swipeMove(a);break;case"end":b.swipeEnd(a)}},b.prototype.swipeMove=function(a){var d,e,f,g,h,b=this;return h=void 0!==a.originalEvent?a.originalEvent.touches:null,!b.dragging||h&&1!==h.length?!1:(d=b.getLeft(b.currentSlide),b.touchObject.curX=void 0!==h?h[0].pageX:a.clientX,b.touchObject.curY=void 0!==h?h[0].pageY:a.clientY,b.touchObject.swipeLength=Math.round(Math.sqrt(Math.pow(b.touchObject.curX-b.touchObject.startX,2))),b.options.verticalSwiping===!0&&(b.touchObject.swipeLength=Math.round(Math.sqrt(Math.pow(b.touchObject.curY-b.touchObject.startY,2)))),e=b.swipeDirection(),"vertical"!==e?(void 0!==a.originalEvent&&b.touchObject.swipeLength>4&&a.preventDefault(),g=(b.options.rtl===!1?1:-1)*(b.touchObject.curX>b.touchObject.startX?1:-1),b.options.verticalSwiping===!0&&(g=b.touchObject.curY>b.touchObject.startY?1:-1),f=b.touchObject.swipeLength,b.touchObject.edgeHit=!1,b.options.infinite===!1&&(0===b.currentSlide&&"right"===e||b.currentSlide>=b.getDotCount()&&"left"===e)&&(f=b.touchObject.swipeLength*b.options.edgeFriction,b.touchObject.edgeHit=!0),b.options.vertical===!1?b.swipeLeft=d+f*g:b.swipeLeft=d+f*(b.$list.height()/b.listWidth)*g,b.options.verticalSwiping===!0&&(b.swipeLeft=d+f*g),b.options.fade===!0||b.options.touchMove===!1?!1:b.animating===!0?(b.swipeLeft=null,!1):void b.setCSS(b.swipeLeft)):void 0)},b.prototype.swipeStart=function(a){var c,b=this;return b.interrupted=!0,1!==b.touchObject.fingerCount||b.slideCount<=b.options.slidesToShow?(b.touchObject={},!1):(void 0!==a.originalEvent&&void 0!==a.originalEvent.touches&&(c=a.originalEvent.touches[0]),b.touchObject.startX=b.touchObject.curX=void 0!==c?c.pageX:a.clientX,b.touchObject.startY=b.touchObject.curY=void 0!==c?c.pageY:a.clientY,void(b.dragging=!0))},b.prototype.unfilterSlides=b.prototype.slickUnfilter=function(){var a=this;null!==a.$slidesCache&&(a.unload(),a.$slideTrack.children(this.options.slide).detach(),a.$slidesCache.appendTo(a.$slideTrack),a.reinit())},b.prototype.unload=function(){var b=this;a(".slick-cloned",b.$slider).remove(),b.$dots&&b.$dots.remove(),b.$prevArrow&&b.htmlExpr.test(b.options.prevArrow)&&b.$prevArrow.remove(),b.$nextArrow&&b.htmlExpr.test(b.options.nextArrow)&&b.$nextArrow.remove(),b.$slides.removeClass("slick-slide slick-active slick-visible slick-current").attr("aria-hidden","true").css("width","")},b.prototype.unslick=function(a){var b=this;b.$slider.trigger("unslick",[b,a]),b.destroy()},b.prototype.updateArrows=function(){var b,a=this;b=Math.floor(a.options.slidesToShow/2),a.options.arrows===!0&&a.slideCount>a.options.slidesToShow&&!a.options.infinite&&(a.$prevArrow.removeClass("slick-disabled").attr("aria-disabled","false"),a.$nextArrow.removeClass("slick-disabled").attr("aria-disabled","false"),0===a.currentSlide?(a.$prevArrow.addClass("slick-disabled").attr("aria-disabled","true"),a.$nextArrow.removeClass("slick-disabled").attr("aria-disabled","false")):a.currentSlide>=a.slideCount-a.options.slidesToShow&&a.options.centerMode===!1?(a.$nextArrow.addClass("slick-disabled").attr("aria-disabled","true"),a.$prevArrow.removeClass("slick-disabled").attr("aria-disabled","false")):a.currentSlide>=a.slideCount-1&&a.options.centerMode===!0&&(a.$nextArrow.addClass("slick-disabled").attr("aria-disabled","true"),a.$prevArrow.removeClass("slick-disabled").attr("aria-disabled","false")))},b.prototype.updateDots=function(){var a=this;null!==a.$dots&&(a.$dots.find("li").removeClass("slick-active").attr("aria-hidden","true"),a.$dots.find("li").eq(Math.floor(a.currentSlide/a.options.slidesToScroll)).addClass("slick-active").attr("aria-hidden","false"))},b.prototype.visibility=function(){var a=this;a.options.autoplay&&(document[a.hidden]?a.interrupted=!0:a.interrupted=!1)},a.fn.slick=function(){var f,g,a=this,c=arguments[0],d=Array.prototype.slice.call(arguments,1),e=a.length;for(f=0;e>f;f++)if("object"==typeof c||"undefined"==typeof c?a[f].slick=new b(a[f],c):g=a[f].slick[c].apply(a[f].slick,d),"undefined"!=typeof g)return g;return a}});
            //]]>
    </script>
    <script type='text/javascript'>
    //<![CDATA[
    function loadCSS(e, t, n) { "use strict"; var i = window.document.createElement("link"); var o = t || window.document.getElementsByTagName("script")[0]; i.rel = "stylesheet"; i.href = e; i.media = "only x"; o.parentNode.insertBefore(i, o); setTimeout(function () { i.media = n || "all" }) }loadCSS("https://maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css");
    //]]>
    </script>
    <script>
      function myFunction() {
        var x = document.getElementById(&quot;myTopnav&quot;);
        if (x.className === &quot;topnav&quot;) {
          x.className += &quot; responsive&quot;;
        } else {
          x.className = &quot;topnav&quot;;
        }
      }
    </script>
    <script>
      function myFunction1() {
        var x = document.getElementById(&quot;myTopnav1&quot;);
        if (x.className === &quot;topnav&quot;) {
          x.className += &quot; responsive&quot;;
        } else {
          x.className = &quot;topnav&quot;;
        }
      }
    </script>
    <script type='text/javascript'>
    //<![CDATA[
    $(document).ready(function(){
        $('.post-body').find('img').each(function(n, image){
        var image = $(image);
        image.parent().css('margin-left',0).css('margin-right',0).css('margin-top',0).css('margin-bottom',0);
        });
    });
    // ]]>
    </script>
    <!--Related Posts with thumbnails Scripts and Styles Start-->
<b:if cond='data:blog.pageType == &quot;item&quot;'>
<script type='text/javascript'>
//<![CDATA[
var relatedTitles=new Array();var relatedTitlesNum=0;var relatedUrls=new Array();var thumburl=new Array();function related_results_labels_thumbs(json){for(var i=0;i<json.feed.entry.length;i++){var entry=json.feed.entry[i];relatedTitles[relatedTitlesNum]=entry.title.$t;try{thumburl[relatedTitlesNum]=entry.gform_foot.url}catch(error){s=entry.content.$t;a=s.indexOf("<img");b=s.indexOf("src=\"",a);c=s.indexOf("\"",b+5);d=s.substr(b+5,c-b-5);if((a!=-1)&&(b!=-1)&&(c!=-1)&&(d!="")){thumburl[relatedTitlesNum]=d}else thumburl[relatedTitlesNum]='https://3.bp.blogspot.com/-SrwqNUjBm7o/W554y7nUN8I/AAAAAAAABCs/E69h3XYqNwsbhJfhnqsYVouAj-0X96XMACLcBGAs/s1600/tak-ada-gambar.png'}for(var k=0;k<entry.link.length;k++){if(entry.link[k].rel=='alternate'){relatedUrls[relatedTitlesNum]=entry.link[k].href;relatedTitlesNum++}}}}function removeRelatedDuplicates_thumbs(){var tmp=new Array(0);var tmp2=new Array(0);var tmp3=new Array(0);for(var i=0;i<relatedUrls.length;i++){if(!contains_thumbs(tmp,relatedUrls[i])){tmp.length+=1;tmp[tmp.length-1]=relatedUrls[i];tmp2.length+=1;tmp3.length+=1;tmp2[tmp2.length-1]=relatedTitles[i];tmp3[tmp3.length-1]=thumburl[i]}}relatedTitles=tmp2;relatedUrls=tmp;thumburl=tmp3}function contains_thumbs(a,e){for(var j=0;j<a.length;j++)if(a[j]==e)return true;return false}function printRelatedLabels_thumbs(){for(var i=0;i<relatedUrls.length;i++){if((relatedUrls[i]==currentposturl)||(!(relatedTitles[i]))){relatedUrls.splice(i,1);relatedTitles.splice(i,1);thumburl.splice(i,1);i--}}var r=Math.floor((relatedTitles.length-1)*Math.random());var i=0;if(relatedTitles.length>0)document.write('<h4>'+relatedpoststitle+'</h4>');document.write('<div style="clear: both;"/><div class="row ">');while(i<relatedTitles.length&&i<20&&i<maxresults){document.write('<div class="col"><a style="text-decoration:none;margin:0 4px 10px 0;float:left;');if(i!=0)document.write('"');else document.write('"');document.write(' href="'+relatedUrls[r]+'"><img class="related_img" src="'+thumburl[r]+'"/><br/><div id="related-title">'+relatedTitles[r]+'</div></div></a>');if(r<relatedTitles.length-1){r++}else{r=0}i++}document.write('</div></div>');relatedUrls.splice(0,relatedUrls.length);thumburl.splice(0,thumburl.length);relatedTitles.splice(0,relatedTitles.length)}
//]]>
</script>
</b:if>
<!--Related Posts with thumbnails Scripts and Styles End-->
  </head>

  <body class='full' id='atas'>
   <b:section class='navbar' id='navbar' maxwidgets='1' name='Navbar' showaddelement='no'>
     <b:widget id='Navbar1' locked='false' title='Navbar' type='Navbar' version='1'>
       <b:includable id='main'>&lt;script type=&quot;text/javascript&quot;&gt;
    function setAttributeOnload(object, attribute, val) {
      if(window.addEventListener) {
        window.addEventListener(&#39;load&#39;,
          function(){ object[attribute] = val; }, false);
      } else {
        window.attachEvent(&#39;onload&#39;, function(){ object[attribute] = val; });
      }
    }
  &lt;/script&gt;
&lt;div id=&quot;navbar-iframe-container&quot;&gt;&lt;/div&gt;
&lt;script type=&quot;text/javascript&quot; src=&quot;https://apis.google.com/js/platform.js&quot;&gt;&lt;/script&gt;
&lt;script type=&quot;text/javascript&quot;&gt;
      gapi.load(&quot;gapi.iframes:gapi.iframes.style.bubble&quot;, function() {
        if (gapi.iframes &amp;&amp; gapi.iframes.getContext) {
          gapi.iframes.getContext().openChild({
              url: &#39;https://draft.blogger.com/navbar.g?targetBlogID\x3d6465428916646986361\x26blogName\x3dJasa+Nikah+Siri+Terdekat+Dari+Lokasi+...\x26publishMode\x3dPUBLISH_MODE_BLOGSPOT\x26navbarType\x3dLIGHT\x26layoutType\x3dLAYOUTS\x26searchRoot\x3dhttps://jasanikahsiriblitar.blogspot.com/search\x26blogLocale\x3din\x26v\x3d2\x26homepageUrl\x3dhttp://jasanikahsiriblitar.blogspot.com/\x26vt\x3d-8125105509401781489&#39;,
              where: document.getElementById(&quot;navbar-iframe-container&quot;),
              id: &quot;navbar-iframe&quot;
          });
        }
      });
    &lt;/script&gt;&lt;script type=&quot;text/javascript&quot;&gt;
(function() {
var script = document.createElement(&#39;script&#39;);
script.type = &#39;text/javascript&#39;;
script.src = &#39;//pagead2.googlesyndication.com/pagead/js/google_top_exp.js&#39;;
var head = document.getElementsByTagName(&#39;head&#39;)[0];
if (head) {
head.appendChild(script);
}})();
&lt;/script&gt;
</b:includable>
     </b:widget>
   </b:section>
    <b:if cond='data:blog.pageType != &quot;index&quot;'>
      <b:if cond='data:blog.pageType != &quot;item&quot; and data:blog.pageType != &quot;static_page&quot;'>
        <b:if cond='data:blog.metaDescription != &quot;&quot;'>
          <meta expr:content='data:blog.metaDescription' name='description'/>
        </b:if>
      </b:if>
    </b:if>
    <div class='body-fauxcolumns'>
      <div class='fauxcolumn-outer body-fauxcolumn-outer'>
        <div class='cap-top'>
          <div class='cap-left'/>
          <div class='cap-right'/>
        </div>
        <div class='fauxborder-left'>
          <div class='fauxborder-right'/>
          <div class='fauxcolumn-inner'>
          </div>
        </div>
        <div class='cap-bottom'>
          <div class='cap-left'/>
          <div class='cap-right'/>
        </div>
      </div>
    </div>
    <div class='content'>
      <div class='content-fauxcolumns'>
        <div class='fauxcolumn-outer content-fauxcolumn-outer'>
          <div class='cap-top'>
            <div class='cap-left'/>
            <div class='cap-right'/>
          </div>
          <div class='fauxborder-left'>
            <div class='fauxborder-right'/>
            <div class='fauxcolumn-inner'>
            </div>
          </div>
          <div class='cap-bottom'>
            <div class='cap-left'/>
            <div class='cap-right'/>
          </div>
        </div>
      </div>
      <div class='content-outer'>
        <div class='content-cap-top cap-top'>
          <div class='cap-left'/>
          <div class='cap-right'/>
        </div>
        <div class='fauxborder-left content-fauxborder-left'>
          <div class='fauxborder-right content-fauxborder-right'/>

          <!-- begin header -->
          <header>
            <div class='header-outer'>
              <div class='header-cap-top cap-top'>
                <div class='cap-left'/>
                <div class='cap-right'/>
              </div>
              <div class='fauxborder-left header-fauxborder-left'>
                <div class='fauxborder-right header-fauxborder-right'/>
                <div class='region-inner header-inner'>
                  <b:section class='header' id='header' maxwidgets='1' name='Header' showaddelement='no'>
                    <b:widget id='Header1' locked='false' title='Jasa Nikah Siri Terdekat Dari Lokasi Saya Murah Tanpa Wali (Header)' type='Header'>
                      <b:widget-settings>
                        <b:widget-setting name='displayUrl'/>
                        <b:widget-setting name='displayHeight'>0</b:widget-setting>
                        <b:widget-setting name='sectionWidth'>-1</b:widget-setting>
                        <b:widget-setting name='useImage'>false</b:widget-setting>
                        <b:widget-setting name='shrinkToFit'>false</b:widget-setting>
                        <b:widget-setting name='imagePlacement'>BEHIND</b:widget-setting>
                        <b:widget-setting name='displayWidth'>0</b:widget-setting>
                      </b:widget-settings>
                      <b:includable id='main'>

  <b:if cond='data:useImage'>
    <b:if cond='data:imagePlacement == &quot;BEHIND&quot;'>
      <!--
      Show image as background to text. You can't really calculate the width
      reliably in JS because margins are not taken into account by any of
      clientWidth, offsetWidth or scrollWidth, so we don't force a minimum
      width if the user is using shrink to fit.
      This results in a margin-width's worth of pixels being cropped. If the
      user is not using shrink to fit then we expand the header.
      -->
      <b:if cond='data:mobile'>
        <div id='header-inner'>
          <div class='titlewrapper' style='background: transparent'>
            <h1 class='title' style='background: transparent; border-width: 0px'>
              <b:include name='title'/>
            </h1>
          </div>
          <b:include name='description'/>
        </div>
      <b:else/>
        <div expr:style='&quot;background-image: url(\&quot;&quot; + data:sourceUrl + &quot;\&quot;); &quot;                      + &quot;background-position: &quot;                      + data:backgroundPositionStyleStr + &quot;; &quot;                      + data:widthStyleStr                      + &quot;min-height: &quot; + data:height                      + &quot;_height: &quot; + data:height                      + &quot;background-repeat: no-repeat; &quot;' id='header-inner'>
          <div class='titlewrapper' style='background: transparent'>
            <h1 class='title' style='background: transparent; border-width: 0px'>
              <b:include name='title'/>
            </h1>
          </div>
          <b:include name='description'/>
        </div>
      </b:if>
    <b:else/>
      <!--Show the image only-->
      <div id='header-inner'>
        <a expr:href='data:blog.homepageUrl' style='display: block'>
          <img expr:alt='data:title' expr:height='data:height' expr:id='data:widget.instanceId + &quot;_headerimg&quot;' expr:src='data:sourceUrl' expr:width='data:width' style='display: block'/>
        </a>
        <!--Show the description-->
        <b:if cond='data:imagePlacement == &quot;BEFORE_DESCRIPTION&quot;'>
          <b:include name='description'/>
        </b:if>
      </div>
    </b:if>
  <b:else/>
    <!--No header image -->
    <div id='header-inner'>
      <div class='titlewrapper'>
        <h1 class='title'>
          <b:include name='title'/>
        </h1>
      </div>
      <b:include name='description'/>
    </div>
  </b:if>
</b:includable>
                      <b:includable id='description'>
  <div class='descriptionwrapper'>
    <p class='description'><span><data:description/></span></p>
  </div>
</b:includable>
                      <b:includable id='title'>
  <b:tag cond='data:blog.url != data:blog.homepageUrl' expr:href='data:blog.homepageUrl' name='a'>
    <data:title/>
  </b:tag>
</b:includable>
                    </b:widget>
                  </b:section>
                </div>
              </div>
              <div class='header-cap-bottom cap-bottom'>
                <div class='cap-left'/>
                <div class='cap-right'/>
              </div>
            </div>
          </header>
          <!-- end header -->

          <!-- menu -->
          <div class='tabs-outer'>
            <div class='tabs-cap-top cap-top'>
              <div class='cap-left'/>
              <div class='cap-right'/>
            </div>
            <div class='fauxborder-left tabs-fauxborder-left'>
              <div class='fauxborder-right tabs-fauxborder-right'/>
              <div class=' tabs-inner'>
                <b:section class='tabs' id='crosscol' maxwidgets='1' name='Menu' showaddelement='no'>
                  <b:widget id='PageList1' locked='false' title='Pages' type='PageList' version='1'>
                    <b:widget-settings>
                      <b:widget-setting name='pageListJson'>{}</b:widget-setting>
                      <b:widget-setting name='homeTitle'>Beranda</b:widget-setting>
                    </b:widget-settings>
                    <b:includable id='main'>
                      <b:if cond='data:title != &quot;&quot;'>
                        <h2>
                          <data:title/>
                        </h2>
                      </b:if>
                      <div class='widget-content'>
                        <b:if cond='data:mobile'>
                          <select expr:id='data:widget.instanceId + &quot;_select&quot;'>
                            <b:loop values='data:links' var='link'>
                              <b:if cond='data:link.isCurrentPage'>
                                <option expr:value='data:link.href' selected='selected'>
                                  <data:link.title/>
                                </option>
                                <b:else/>
                                <option expr:value='data:link.href'>
                                  <data:link.title/>
                                </option>
                              </b:if>
                            </b:loop>
                          </select>
                          <span class='pagelist-arrow'>
                            &amp;#9660;
                          </span>
                          <b:else/>
                          <ul class='topnav' id='myTopnav'>
                            <b:loop values='data:links' var='link'>
                              <b:if cond='data:link.isCurrentPage'>
                                <li class='selected'>
                                  <a expr:href='data:link.href'>
                                    <data:link.title/>
                                  </a>
                                </li>
                                <b:else/>
                                <li>
                                  <a expr:href='data:link.href'>
                                    <data:link.title/>
                                  </a>
                                </li>
                              </b:if>
                            </b:loop>

                            <li class='icon'>
                              <a href='javascript:void(0);' onclick='myFunction()'>
                                <i aria-hidden='true' class='fa fa-bars'/>
                              </a>
                            </li>
                          </ul>
                        </b:if>
                        <b:include name='quickedit'/>
                      </div>
                    </b:includable>
                  </b:widget>
                </b:section>

                <!-- sementara dimatikan -->
                <!--b:section class='tabs' id='crosscol-overflow' name='Cross-Column 2' showaddelement='no'/-->
                <!-- end mati -->
              </div>
            </div>
            <div class='tabs-cap-bottom cap-bottom'>
              <div class='cap-left'/>
              <div class='cap-right'/>
            </div>
          </div>
          <!-- end menu -->

          <!-- HEADER + MENU -->
          <div class='header-menu'>
          	<div class='wrap-hm row group'>

							<div class='headernya col kolom13'>
								<!-- begin header -->
								<header>
									<div class='header-outer'>
										<div class='header-cap-top cap-top'>
											<div class='cap-left'/>
											<div class='cap-right'/>
										</div>
										<div class='fauxborder-left header-fauxborder-left'>
											<div class='fauxborder-right header-fauxborder-right'/>
											<div class='region-inner header-inner'>
												<b:section class='header' id='header2' maxwidgets='1' name='Header2' showaddelement='no'/>
											</div>
										</div>
										<div class='header-cap-bottom cap-bottom'>
											<div class='cap-left'/>
											<div class='cap-right'/>
										</div>
									</div>
								</header>
								<!-- end header -->
							</div>

							<div class='col kolom23'>
							<div class='menunya'>
								<!-- menu -->
								<div class='tabs-outer'>
									<div class='tabs-cap-top cap-top'>
										<div class='cap-left'/>
										<div class='cap-right'/>
									</div>
									<div class='fauxborder-left tabs-fauxborder-left'>
										<div class='fauxborder-right tabs-fauxborder-right'/>
										<div class=' tabs-inner'>
											<b:section class='tabs' id='crosscol1' maxwidgets='1' name='Menu2' showaddelement='no'/>

											<!-- sementara dimatikan -->
											<!--b:section class='tabs' id='crosscol-overflow' name='Cross-Column 2' showaddelement='no'/-->
											<!-- end mati -->
										</div>
									</div>
									<div class='tabs-cap-bottom cap-bottom'>
										<div class='cap-left'/>
										<div class='cap-right'/>
									</div>
								</div>
								<!-- end menu -->
								</div>
							</div>

          	</div>
          </div>
          <!-- END HEADER + MENU -->

          <!-- kondisi hanya tampil dihalaman depan saja -->
          <b:if cond='data:blog.url == data:blog.homepageUrl'>

              <!-- ################### -->
              <!-- COVER -->
              <!-- ################### -->
              <div class='cover'>
                <b:section class='w-cover' id='Cover' maxwidgets='1' showaddelement='yes'>
                  <b:widget id='HTML1' locked='false' title='' type='HTML' version='1'>
                    <b:widget-settings>
                      <b:widget-setting name='content'><![CDATA[<div class="cover2">
    <div class="row group">
        <div class="col cover-kolom12">
            <h2>Jasa Nikah Siri Terdekat Dari Lokasi Saya Murah Tanpa Wali</h2>
            <p>Jasa Nikah Siri Terdekat Dari Lokasi Saya- Agama islam pun udah memastikan kalau stu-satunya jalan buat penuhi kepentingan biologis manusia yaitu hanya cukup pernikahn, pernikahan yaitu satu soal yang sangat bagus apabila kita lebih mengamati kandungan pengertian terkait persoalan pernikahan ini.

Di al-Qur'an udah diperjelas kalau pernikahan nyatanya pun bisa bawa kenyamanan dalam kehidupan satu orang (litaskunu ilaiha).

Ini bermakna pernikahan kenyataannya bukanlah sekedar selaku media pendistribusian kepentingan seks akan tetapi lebih dari pada itu pernikahan pun janjikan perdamaian hidup buat manusia di mana tiap-tiap manusia bisa membentuk surga dunia di dalamnya.

Segalanya itu bakal terjadi seandainya pernikahan itu sungguh-sungguh di lakoni dengan sesuai sama lajur yang udah ditentukan islam dapat mengabari Jasa Nikah Siri Terdekat Dari Lokasi Saya
 Klik Tombol dibawah ini langsung tersambung dengan kami :</p>
            <a class="btn btn-merah" href="https://api.whatsapp.com/send?phone=6281392175464&amp;text=Assalamu'alaikum.wr.wb%20Pak Ustadz%20Saya%20Dari%20Kabupaten:...........%20Syarat%20dan%20Biaya%20Nikah%20Siri%20Berapa?%3F">Whatsapp</a>
<a class="btn btn-merah" href="tel:+6281392175464">Telepone</a>
        </div>
        <div class="col cover-kolom22 txt-center">
            <img src="https://1.bp.blogspot.com/-4Vf7WXgislA/YGvmOBQOrRI/AAAAAAAAE2I/0YNj_Vd-GU0qESYqjLiLfVfAMpvf50GpgCLcBGAsYHQ/s0/18034ab5-karikatur-kartun-akad-nikah-300x250.jpg" alt="jasa pembuatan website" />
        </div>
    </div>
</div>]]></b:widget-setting>
                    </b:widget-settings>
                    <b:includable id='main'>
                      <div class='widget-content'>
                            <data:content/>
                      </div>

                      <b:include name='quickedit'/>
                    </b:includable>
                  </b:widget>
                </b:section>
              </div>
              <!-- ################### -->
              <!-- END COVER -->
              <!-- ################### -->


              <!-- ################### -->
              <!-- PEMISAH 1 -->
              <!-- ################### -->
              <div class='aroodam-content-1'>
                <b:section class='box-konten' id='Pemisah1' maxwidgets='' showaddelement='yes'>
                  <b:widget id='HTML2' locked='false' title='' type='HTML' version='1'>
                    <b:widget-settings>
                      <b:widget-setting name='content'><![CDATA[<div class="feat-33">
    <div class="row group ">
        <div class="feat-list">
            <div class="col kolom23">
                <div class="head-feat">
                    <h3>Penjelasan Nikah Siri</h3>
                    <p>Perkahwinan atau nikah menurut bahasa merupakan berbaur serta kumpul.

Menurut makna syarak juga merupakan ijab serta qabul (‘aqad) yang menghalalkan persetubuhan di antara lelaki serta wanita yang disampaikan oleh beberapa kata yang tunjukkan nikah, menurut ketetapan yang dipastikan oleh Islam.

Pengucapan zawaj dipakai di al-Quran dengan maksud pasangan dalam pemanfaatannya pengucapan ini dengan maksud perkahwinan Allah s.w.t. bikin manusia itu berpasang-pasangan, menghalalkan mengharamkan zina serta perkahwinan.

Tentang hal nikah menurut syari'at nikah pun bermakna akad. Sementara itu penjelasan interaksi tubuh itu cuman metafora saja.

Pernikahan yaitu sunnah karuniah yang seandainya dikerjakan bakal memperoleh pahala namun seandainya tak dikerjakan tak mendapat dosa namun dimakruhkan sebab tak meng ikuti sunnah rosul.

Makna dari Siri pernikahan di tempat ini yaitu menyatunya dua insane dengan macam tidak sama ialah laki laki serta wanita yang merajut satu ikatan dengan janji atau persetujuan.

Satu pernikahan miliki arah ialah pengin menciptakan keluarga yang sakinah mawaddah warohmah dan pengin mendapat trah yang solihah. Trah berikut ini yang Jasa Nikah Siri terus diinginkan oleh tiap orang yang udah menikah sebab trah yaitu angkatan buat orang tuanya.
            </p></div>
        </div>
  <a href="https://www.nikahsiri.id/2022/12/jasa-nikah-siri-hulu-sungai.html">Nikah Siri Hulu Sungai</a>
 <a href="https://www.nikahsiri.id/2022/12/nikah-siri-kotabaru.html">Nikah Siri Kota Baru</a>
 <a href="https://www.nikahsiri.id/2022/12/nikah-siri-banjarbaru.html">Nikah Siri Banjarbaru</a>
 <a href="https://www.nikahsiri.id/2022/12/nikah-siri-banjarmasin.html">Nikah Siri Banjarmasin</a>
 <a href="https://www.nikahsiri.id/2022/11/nikah-siri-singapura.html">Nikah Siri Singapura</a>
 <a href="https://www.nikahsiri.id/2022/11/nikah-siri-barru.html">Nikah Siri Barru</a>
 <a href="https://www.nikahsiri.id/2022/11/nikah-siri-janeponto.html">Nikah Siri Janeponto</a>
 <a href="https://www.nikahsiri.id/2022/11/nikah-siri-bantaeng.html">Nikah Siri bantaeng</a>
 <a href="https://www.nikahsiri.id/2022/11/nikah-siri-takalar.html">Nikah Siri Takalar</a>
 <a href="https://www.nikahsiri.id/2022/07/jasa-nikah-siri-tulungagung.html">Nikah Siri Tulungagung</a>
 <a href="https://www.nikahsiri.id/2021/10/nikah-siri-pematangsiantar.html">Nikah Siri Pematangsiantar</a>
 <a href="https://www.nikahsiri.id/2021/10/nikah-siri-tapanuli.html">Nikah Siri Tapanuli</a>
 <a href="https://www.nikahsiri.id/2021/10/nikah-siri-nias.html">Nikah Siri nias</a>
 <a href="https://www.nikahsiri.id/2021/10/nikah-siri-labuhanbatu.html">Nikah Siri labuhanbatu</a>
 <a href="https://www.nikahsiri.id/2021/09/nikah-siri-ketapang.html">Nikah Siri ketapang</a>
 <a href="https://www.nikahsiri.id/2021/09/nikah-siri-kutai.html">Nikah Siri kutai</a>
 <a href="https://www.nikahsiri.id/2021/09/nikah-siri-balikpapan.html">Nikah Siri balikpapan</a>
 <a href="https://www.nikahsiri.id/2021/09/jasa-nikah-siri-sambas.html">Nikah Siri sambas</a>
 <a href="https://www.nikahsiri.id/2021/09/jasa-nikah-siri-halmahera.html">Nikah Siri halmahera</a>
 <a href="https://www.nikahsiri.id/2021/09/jasa-nikah-siri-kolaka.html">Nikah Siri kolaka</a>
 <a href="https://www.nikahsiri.id/2021/08/jasa-nikah-siri-konawe.html">Nikah Siri konawe</a>
 <a href="https://www.nikahsiri.id/2021/08/jasa-nikah-siri-bone.html">Nikah Siri bone</a>
 <a href="https://www.nikahsiri.id/2021/08/jasa-nikah-siri-gowa.html">Nikah Siri gowa</a>
 <a href="https://www.nikahsiri.id/2021/08/jasa-nikah-siri-pasaman.html">Nikah Siri pasaman</a>
 <a href="https://www.nikahsiri.id/2021/08/jasa-nikah-siri-solok.html">Nikah Siri solok</a>
 <a href="https://www.nikahsiri.id/2021/07/jasa-nikah-siri-dharmasraya.html">Nikah Siri dharmasraya</a>
 <a href="https://www.nikahsiri.id/2021/07/jasa-nikah-siri-agam.html">Nikah Siri agam</a>
 <a href="https://www.nikahsiri.id/2021/07/jasa-nikah-siri-asahan.html">Nikah Siri asahan</a>
 <a href="https://www.nikahsiri.id/2021/07/nikah-siri-deli-serdang.html">Nikah Siri deli serdang</a>
 <a href="https://www.nikahsiri.id/2021/07/jasa-nikah-siri-simalungun.html">Nikah Siri simalungun</a>
 <a href="https://www.nikahsiri.id/2021/07/jasa-nikah-siri-langkat.html">Nikah Siri langkat</a>
 <a href="https://www.nikahsiri.id/2021/07/jasa-nikah-siri-dumai.html">Nikah Siri dumai</a>
 <a href="https://www.nikahsiri.id/2021/07/jasa-nikah-siri-rokan.html">Nikah Siri rokan</a>
 <a href="https://www.nikahsiri.id/2021/07/jasa-nikah-siri-kampar.html">Nikah Siri kampar</a>
 <a href="https://www.nikahsiri.id/2021/06/nikah-siri-indragiri-hilir.html">Nikah Siri indragiri</a>
 <a href="https://www.nikahsiri.id/2021/06/jasa-nikah-siri-palu.html">Nikah Siri palu</a>
 <a href="https://www.nikahsiri.id/2021/06/jasa-nikah-siri-manokrawi.html">Nikah Siri manokrawi</a>
 <a href="https://www.nikahsiri.id/2021/05/jasa-nikah-siri-palangkaraya.html">Nikah Siri palangkaraya</a>
 <a href="https://www.nikahsiri.id/2021/05/jasa-nikah-siri-kupang.html">Nikah Siri kupang</a>
 <a href="https://www.nikahsiri.id/2021/05/jasa-nikah-siri-malaysia-100-terpercaya.html">Nikah Siri malaysia</a>
 <a href="https://www.nikahsiri.id/2021/05/jasa-nikah-siri-nganjuk.html">Nikah Siri nganjuk</a>
 <a href="https://www.nikahsiri.id/2021/05/jasa-nikah-siri-lumajang.html">Nikah Siri lumajang</a>
 <a href="https://www.nikahsiri.id/2021/04/jasa-nikah-siri-serang.html">Nikah Siri serang</a>
 <a href="https://www.nikahsiri.id/2021/04/jasa-nikah-siri-cilegon.html">Nikah Siri cilegon</a>
 <a href="https://www.nikahsiri.id/2021/04/jasa-nikah-siri-karawang.html">Nikah Siri karawang</a>
 <a href="https://www.nikahsiri.id/2021/04/jasa-nikah-siri-jayapura.html">Nikah Siri jayapura</a>
 <a href="https://www.nikahsiri.id/2021/04/jasa-nikah-siri-gorontalo.html">Nikah Siri gorontalo</a>
 <a href="https://www.nikahsiri.id/2021/03/nikah-siri-ciamis.html">Nikah Siri ciamis</a>
 <a href="https://www.nikahsiri.id/2021/03/nikah-siri-majalengka.html">Nikah Siri majalengka</a>
 <a href="https://www.nikahsiri.id/2021/03/nikah-siri-garut.html">Nikah Siri garut</a>
 <a href="https://www.nikahsiri.id/2021/03/nikah-siri-sumedang.html">Nikah Siri sumedang</a>
 <a href="https://www.nikahsiri.id/2021/03/nikah-siri-banjar.html">Nikah Siri banjar</a>
 <a href="https://www.nikahsiri.id/2021/03/nikah-siri-tasikmalaya.html">Nikah Siri tasikmalaya</a>
 <a href="https://www.nikahsiri.id/2021/03/nikah-siri-jepara.html">Nikah Siri jepara</a>
 <a href="https://www.nikahsiri.id/2021/03/nikah-siri-kudus.html">Nikah Siri kudus</a>
 <a href="https://www.nikahsiri.id/2021/03/nikah-siri-magetan.html">Nikah Siri magetan</a>
 <a href="https://www.nikahsiri.id/2021/03/nikah-siri-ngawi.html">Nikah Siri ngawi</a>
 <a href="https://www.nikahsiri.id/2021/03/nikah-siri-madiun.html">Nikah Siri madiun</a>
 <a href="https://www.nikahsiri.id/2021/03/nikah-siri-trenggalek.html">Nikah Siri trenggalek</a>
 <a href="https://www.nikahsiri.id/2021/03/nikah-siri-pasuruan.html">Nikah Siri pasuruan</a>
 <a href="https://www.nikahsiri.id/2021/03/nikah-siri-malang.html">Nikah Siri malang</a>
 <a href="https://www.nikahsiri.id/2021/02/jasa-nikah-siri-online.html">Nikah Siri online</a>
 <a href="https://www.nikahsiri.id/2021/02/jasa-nikah-siri.html">Jasa Nikah Siri</a>
 <a href="https://www.nikahsiri.id/2021/01/nikah-siri-yogyakarta.html">Nikah Siri Jogja</a>
<a href="https://www.nikahsiri.id/2021/01/nikah-siri-yogyakarta.html">Nikah Siri Yogyakarta</a>
 <a href="https://www.nikahsiri.id/2021/01/nikah-siri-subang.html">Nikah Siri subang</a>
 <a href="https://www.nikahsiri.id/2021/01/nikah-siri-sukabumi.html">Nikah Siri sukabumi</a>
 <a href="https://www.nikahsiri.id/2021/01/nikah-siri-kuningan.html">Nikah Siri kuningan</a>
 <a href="https://www.nikahsiri.id/2021/01/nikah-siri-cimahi.html">Nikah Siri cimahi</a>
 <a href="https://www.nikahsiri.id/2021/01/nikah-siri-cianjur.html">Nikah Siri cianjur</a>
 <a href="https://www.nikahsiri.id/2021/01/nikah-siri-purwakarta.html">Nikah Siri purwakarta</a>
 <a href="https://www.nikahsiri.id/2021/01/nikah-siri-bondowoso.html">Nikah Siri bondowoso</a>
 <a href="https://www.nikahsiri.id/2021/01/jasa-nikah-siri-jember.html">Nikah Siri jember</a>
 <a href="https://www.nikahsiri.id/2021/01/nikah-siri-banyuwangi.html">Nikah Siri banyuwangi</a>
 <a href="https://www.nikahsiri.id/2021/01/nikah-siri-pamekasan.html">Nikah Siri pamekasan</a>
 <a href="https://www.nikahsiri.id/2021/01/nikah-siri-sampang.html">Nikah Siri sampang</a>
 <a href="https://www.nikahsiri.id/2021/01/nikah-siri-pacitan.html">Nikah Siri pacitan</a>
 <a href="https://www.nikahsiri.id/2021/01/jasa-nikah-siri-indramayu.html">Nikah Siri indramayu</a>
 <a href="https://www.nikahsiri.id/2021/01/jasa-nikah-siri-cirebon.html">Nikah Siri cirebon</a>
 <a href="https://www.nikahsiri.id/2020/12/jasa-nikah-siri-sidoarjo.html">Nikah Siri sidoarjo</a>
 <a href="https://www.nikahsiri.id/2020/12/nikah-siri-situbondo.html">Nikah Siri situbondo</a>
 <a href="https://www.nikahsiri.id/2020/12/jasa-nikah-siri-batu.html">Nikah Siri batu</a>
 <a href="https://www.nikahsiri.id/2020/12/jasa-nikah-siri-blitar.html">Nikah Siri blitar</a>
 <a href="https://www.nikahsiri.id/2020/12/nikah-siri-sumenep.html">Nikah Siri sumenep</a>
 <a href="https://www.nikahsiri.id/2020/12/nikah-siri-tuban.html">Nikah Siri tuban</a>
 <a href="https://www.nikahsiri.id/2020/12/jasa-nikah-siri-kediri.html">Nikah Siri kediri</a>
 <a href="https://www.nikahsiri.id/2020/12/nikah-siri-bogor.html">Nikah Siri bogor</a>
 <a href="https://www.nikahsiri.id/2020/12/nikah-siri-bangkalan.html">Nikah Siri bangkalan</a>
 <a href="https://www.nikahsiri.id/2020/12/nikah-siri-bekasi.html">Nikah Siri bekasi</a>
 <a href="https://www.nikahsiri.id/2020/12/nikah-siri-wonogiri.html">Nikah Siri wonogiri</a>
 <a href="https://www.nikahsiri.id/2020/12/nikah-siri-purworejo.html">Nikah Siri purworejo</a>
 <a href="https://www.nikahsiri.id/2020/12/nikah-siri-purbalingga.html">Nikah Siri purbalingga</a>
 <a href="https://www.nikahsiri.id/2020/12/nikah-siri-pemalang.html">Nikah Siri pemalang</a>
 <a href="https://www.nikahsiri.id/2020/11/nikah-siri-demak.html">Nikah Siri demak</a>
 <a href="https://www.nikahsiri.id/2020/11/nikah-siri-banjarnegara.html">Nikah Siri banjarnegara</a>
 <a href="https://www.nikahsiri.id/2020/11/nikah-siri-banyumas.html">Nikah Siri banyumas</a>
 <a href="https://www.nikahsiri.id/2020/10/jasa-nikah-siri-batam.html">Nikah Siri batam</a>
 <a href="https://www.nikahsiri.id/2020/10/jasa-nikah-siri-lahat.html">Nikah Siri lahat</a>
 <a href="https://www.nikahsiri.id/2020/10/jasa-nikah-siri-lubuklinggau.html">Nikah Siri lubuklinggau</a>
 <a href="https://www.nikahsiri.id/2020/10/jasa-nikah-siri-ogan-komering-ilir.html">Nikah Siri Oki</a>
 <a href="https://www.nikahsiri.id/2020/10/jasa-nikah-siri-banyuasin.html">Nikah Siri banyuasin</a>
 <a href="https://www.nikahsiri.id/2020/10/jasa-nikah-siri-prabumulih.html">Nikah Siri prabumulih</a>
 <a href="https://www.nikahsiri.id/2020/05/jasa-nikah-siri-makassar.html">Nikah Siri makassar</a>
 <a href="https://www.nikahsiri.id/2020/04/jasa-nikah-siri-lampung.html">Nikah Siri lampung</a>
 <a href="https://www.nikahsiri.id/2020/03/jasa-nikah-siri-riau.html">Nikah Siri riau</a>
 <a href="https://www.nikahsiri.id/2020/02/jasa-nikah-siri-padang.html">Nikah Siri padang</a>
 <a href="https://www.nikahsiri.id/2020/02/jasa-nikah-siri-banda-aceh.html">Nikah Siri aceh</a>
 <a href="https://www.nikahsiri.id/2020/01/jasa-nikah-siri-samarinda.html">Nikah Siri samarinda</a>
 <a href="https://www.nikahsiri.id/2020/01/jasa-nikah-siri-manado.html">Nikah Siri manado</a>
 <a href="https://www.nikahsiri.id/2020/01/jasa-nikah-siri-palembang-wa.html">Nikah Siri palembang</a>
 <a href="https://www.nikahsiri.id/2019/12/jasa-nikah-siri-medan.html">Nikah Siri medan</a>
 <a href="https://www.nikahsiri.id/2019/12/jasa-nikah-siri-jambi.html">Nikah Siri jambi</a>
 <a href="https://www.nikahsiri.id/2019/12/jasa-nikah-siri-pontianak.html">Nikah Siri pontianak</a>
 <a href="https://www.nikahsiri.id/2019/12/jasa-nikah-siri-pekanbaru.html">Nikah Siri pekanbaru</a>
 <a href="https://www.nikahsiri.id/2019/07/jasa-nikah-siri-bandung.html">Nikah Siri bandung</a>
 <a href="https://www.nikahsiri.id/2019/05/jasa-nikah-siri-cilacap.html">Nikah Siri cilacap</a>
 <a href="https://www.nikahsiri.id/2019/05/jasa-nikah-siri-kebumen.html">Nikah Siri kebumen</a>
 <a href="https://www.nikahsiri.id/2019/05/jasa-nikah-siri-gresik.html">Nikah Siri gresik</a>
 <a href="https://www.nikahsiri.id/2019/03/jasa-penghulu-nikah-siri-blora.html">Nikah Siri blora</a>
 <a href="https://www.nikahsiri.id/2019/03/jasa-penghulu-nikah-siri-rembang.html">Nikah Siri rembang</a>
 <a href="https://www.nikahsiri.id/2019/03/jasa-penghulu-nikah-siri-mojokerto.html">Nikah Siri mojokerto</a>
 <a href="https://www.nikahsiri.id/2019/03/jasa-penghulu-nikah-siri-bojonegoro.html">Nikah Siri bojonegoro</a>
 <a href="https://www.nikahsiri.id/2019/02/jasa-penghulu-nikah-siri-ponorogo.html">Nikah Siri ponorogo</a>
 <a href="https://www.nikahsiri.id/2019/02/jasa-penghulu-nikah-siri-pati.html">Nikah Siri pati</a>
 <a href="https://www.nikahsiri.id/2019/02/jasa-penghulu-nikah-siri-depok.html">Nikah Siri depok</a>
 <a href="https://www.nikahsiri.id/2019/01/jasa-penghulu-nikah-siri-bengkulu.html">Nikah Siri bengkulu</a>
 <a href="https://www.nikahsiri.id/2019/01/jasa-penghulu-nikah-siri-temanggung.html">Nikah Siri temanggung</a>
 <a href="https://www.nikahsiri.id/2019/01/jasa-penghulu-nikah-siri-salatiga.html">Nikah Siri salatiga</a>
 <a href="https://www.nikahsiri.id/2019/01/jasa-penghulu-nikah-siri-sragen.html">Nikah Siri sragen</a>
 <a href="https://www.nikahsiri.id/2019/01/jasa-penghulu-nikah-siri-sukoharjo.html">Nikah Siri sukoharjo</a>
 <a href="https://www.nikahsiri.id/2019/01/jasa-penghulu-nikah-siri-boyolali.html">Nikah Siri boyolali</a>
 <a href="https://www.nikahsiri.id/2018/12/jasa-penghulu-nikah-siri-batang.html">Nikah Siri batang</a>
 <a href="https://www.nikahsiri.id/2018/12/jasa-penghulu-nikah-siri-pekalongan.html">Nikah Siri pekalongan</a>
 <a href="https://www.nikahsiri.id/2018/12/jasa-penghulu-nikah-siri-brebes.html">Nikah Siri brebes</a>
 <a href="https://www.nikahsiri.id/2018/12/jasa-penghulu-nikah-siri-tegal.html">Nikah Siri tegal</a>
 <a href="https://www.nikahsiri.id/2018/12/jasa-penghulu-nikah-siri-wonosari.html">Nikah Siri wonosari</a>
 <a href="https://www.nikahsiri.id/2018/12/jasa-penghulu-nikah-siri-kulonprogo.html">Nikah Siri kulonprogo</a>
 <a href="https://www.nikahsiri.id/2018/12/jasa-penghulu-nikah-siri-semarang.html">Nikah Siri semarang</a>
 <a href="https://www.nikahsiri.id/2018/11/jasa-nikah-siri-bali.html">Nikah Siri bali</a>
 <a href="https://www.nikahsiri.id/2018/11/jasa-nikah-siri-kendal.html">Nikah Siri kendal</a>
 <a href="https://www.nikahsiri.id/2018/11/jasa-nikah-siri-purwodadi-karanganyar.html">Nikah Siri purwodadi</a>
<a href="https://www.nikahsiri.id/2018/11/jasa-nikah-siri-purwodadi-karanganyar.html">Nikah Siri Karanganyar</a>
 <a href="https://www.nikahsiri.id/2018/11/jasa-nikah-siri-jombang-lamongan.html">Nikah Siri jombang</a>
<a href="https://www.nikahsiri.id/2018/11/jasa-nikah-siri-jombang-lamongan.html">Nikah Siri lamongan</a>
 <a href="https://www.nikahsiri.id/2018/11/nikah-siri-probolinggo.html">Nikah Siri probolinggo</a>
 <a href="https://www.nikahsiri.id/2018/11/jasa-nikah-siri-surabaya.html">Nikah Siri surabaya</a>
 <a href="https://www.nikahsiri.id/2018/10/nikah-siri-wonosobo.html">Nikah Siri wonosobo</a>
 <a href="https://www.nikahsiri.id/2018/10/jasa-nikah-siri-klaten.html">Nikah Siri klaten</a>
 <a href="https://www.nikahsiri.id/2018/10/jasa-penghulu-nikah-siri-tangerang.html">Nikah Siri tangerang</a>
 <a href="https://www.nikahsiri.id/2018/10/jasa-penghulu-nikah-siri-solo.html">Nikah Siri solo</a>
 <a href="https://www.nikahsiri.id/2018/10/jasa-penghulu-nikah-siri-purwokerto.html">Nikah Siri purwokerto</a>
 <a href="https://www.nikahsiri.id/2018/10/jasa-penghulu-nikah-siri-magelang.html">Nikah Siri magelang</a>
 <a href="https://www.nikahsiri.id/2018/10/jasa-nikah-siri-jakarta.html">Nikah Siri jakarta</a>

</div></div></div>]]></b:widget-setting>
                    </b:widget-settings>
                    <b:includable id='main'>
                      <div class='widget-content'>
                        <data:content/>
                      </div>

                      <b:include name='quickedit'/>
                    </b:includable>
                  </b:widget>
                </b:section>
              </div>

              <!-- ################### -->
              <!-- Features -->
              <!-- ################### -->
              <div class='aroodam-content-2'>
                <b:section class='box-konten' id='Features' maxwidgets='' showaddelement='yes'>
                  <b:widget id='HTML3' locked='false' title='' type='HTML' version='1'>
                    <b:widget-settings>
                      <b:widget-setting name='content'><![CDATA[<div class="feat-5">
    <div class="head-feat txt-center">
        <h2>Makna Jasa Nikah Siri Terdekat Dari Lokasi Saya</h2>
        <p class="txt-caption">Inilah 4 Alasan Jasa Nikah Siri Terdekat Dari Lokasi dan Tanpa Wali.</p>
    </div>
    <div class="row group ">
        <div class="col kolom13 txt-center">
            <img src="https://4.bp.blogspot.com/-nYu0gvUce9k/WHy9j5x3xFI/AAAAAAAAADs/7J7vjiqsqVAiIDRXZ6urLwW5v14O5ITbACLcB/s1600/1483968915_icon-57.png" alt="" />
        </div>
        <div class="col kolom13">
            <div class="feat-list">
                <h3>Buat Penuhi Tuntutan Insting Manusia Yang Asasi</h3>
                <p>Perkawinan Nikah Siri yaitu fitrah manusia, jadi jalan yang resmi buat penuhi kepentingan ini ialah dengan aqad nikah (lewat level perkawinan), bukan dengan benar-benar kotor memuakkan seperti beberapa cara orang kini secara menjalin cinta, kumpul kebo, melacur, berzina, lesbi, homo, dan sebagainya yang udah keluar batas serta diharamkan oleh Islam..</p>
            </div>
            <div class="feat-list">
                <h3> Buat Memagari Ahlak Yang Baik</h3>
                <p>Tujuan inti dari disyari'atkannya Nikah Siri dalam Islam salah satunya merupakan buat memagari martabat manusia dari tindakan kotor serta bengis, yang udah turunkan serta meninabobokan martabat manusia yang luhur.

Islam menyaksikan perkawinan serta penciptaan keluarga selaku media efefktif buat memiara pemuda serta pemudi dari kerusakan, serta buat perlindungan penduduk dari kericuhan..</p>
            </div>
        </div>
        <div class="col kolom13">
            <div class="feat-list">
                <h3>Buat Tegakkan Rumah Tangga Yang Islami</h3>
                <p>Dalam Al-Qur'an dijelaskan kalau Islam membetulkan terdapatnya Thalaq (perpisahan), apabila suami istri sudah tak bisa kembali tegakkan batasan-batas Allah,.</p>
            </div>
            <div class="feat-list">
                <h3>Nikah Siri Dapat melindungi</h3>
                <p>Jasa Nikah Siri Tanpa Wali kebersinambungan hidup manusia di jalan berkembang berketurunan serta biak.
b) Dapat melindungi suami istri tenggelam dalam tindakan hina serta dapat membatasi syahwat seta mengendalikan pandangan dari suatu yang diharamkan.
c) Dapat merehatkan serta menyejukkan jiwa denagn trik hanya duduk serta bencrengkramah dengan pujaan hatiannya.
d) Dapat membikin wanita mengerjakan pekerjaannya sesuai sama kelakuan kewanitaan yang dicetak.
.</p>
            </div>
        </div>
    </div>
</div>]]></b:widget-setting>
                    </b:widget-settings>
                    <b:includable id='main'>
                      <div class='widget-content'>
                            <data:content/>
                      </div>

                      <b:include name='quickedit'/>
                    </b:includable>
                  </b:widget>
                </b:section>
              </div>

              <!-- ################### -->
              <!-- PEMISAH 2 -->
              <!-- ################### -->
              <div class='aroodam-content-3'>
                <b:section class='box-konten' id='Pemisah2' maxwidgets='' showaddelement='yes'/>
              </div>

              <!-- ################### -->
              <!-- TESTIMONI -->
              <!-- ################### -->
              <div class='aroodam-content-4'>
                <b:section class='box-konten' id='Testimoni' maxwidgets='' showaddelement='yes'/>
              </div>

              <!-- ################### -->
              <!-- PEMISAH 3 -->
              <!-- ################### -->
              <div class='aroodam-content-5'>
                <b:section class='box-konten' id='Pemisah3' maxwidgets='' showaddelement='yes'/>
              </div>

              <!-- ################### -->
              <!-- CALL TO ACTION -->
              <!-- ################### -->
              <div class='aroodam-content-6'>
                <b:section class='box-konten' id='CallToAction' maxwidgets='' showaddelement='yes'>
                  <b:widget id='HTML7' locked='false' title='' type='HTML' version='1'>
                    <b:widget-settings>
                      <b:widget-setting name='content'><![CDATA[<div class="cta-16">
    <div class="row group txt-center">
        <div class="head-feat">
            <h2>Hubungi Kami Sekarang Juga</h2>
            <p class="txt-caption">Anda Bisa Menghubungi Kami Lewat WA/Tlp, Klik Tombol Di Bawah ini :</p>
        </div>
         <a class="btn btn-merah" href="https://api.whatsapp.com/send?phone=6281392175464&amp;text=Assalamu'alaikum.wr.wb%20Pak Ustadz%20Syarat%20dan%20Biayanya%2C%20Apasaja%20dan%20Berapa?%3F">Whatsapp</a>
<a class="btn btn-merah" href="tel:+6281392175464">Telepone</a>
        </div>
        </div>]]></b:widget-setting>
                    </b:widget-settings>
                    <b:includable id='main'>
                      <div class='widget-content'>
                            <data:content/>
                      </div>

                      <b:include name='quickedit'/>
                    </b:includable>
                  </b:widget>
                </b:section>
              </div>

              <!-- ################### -->
              <!-- PEMISAH 4 -->
              <!-- ################### -->
              <div class='aroodam-content-7'>
                <b:section class='box-konten' id='Pemisah4' maxwidgets='' showaddelement='yes'/>
              </div>

              <!-- ################### -->
              <!-- FOOTER -->
              <!-- ################### -->
              <div class='aroodam-content-8'>
                <b:section class='box-konten' id='Footer' maxwidgets='' showaddelement='yes'/>
              </div>


          </b:if>
          <!-- kondisi tampil hanya dihalaman depan selesai -->

          <div class='content-inner'>
            <div class='main-outer'>
              <div class='main-cap-top cap-top'>
                <div class='cap-left'/>
                <div class='cap-right'/>
              </div>
              <div class='fauxborder-left main-fauxborder-left'>
                <div class='fauxborder-right main-fauxborder-right'/>
                <div class='region-inner main-inner'>
                  <div class='columns fauxcolumns'>
                    <div class='fauxcolumn-outer fauxcolumn-center-outer'>
                      <div class='cap-top'>
                        <div class='cap-left'/>
                        <div class='cap-right'/>
                      </div>
                      <div class='fauxborder-left'>
                        <div class='fauxborder-right'/>
                        <div class='fauxcolumn-inner'>
                        </div>
                      </div>
                      <div class='cap-bottom'>
                        <div class='cap-left'/>
                        <div class='cap-right'/>
                      </div>
                    </div>
                    <div class='fauxcolumn-outer fauxcolumn-left-outer'>
                      <div class='cap-top'>
                        <div class='cap-left'/>
                        <div class='cap-right'/>
                      </div>
                      <div class='fauxborder-left'>
                        <div class='fauxborder-right'/>
                        <div class='fauxcolumn-inner'>
                        </div>
                      </div>
                      <div class='cap-bottom'>
                        <div class='cap-left'/>
                        <div class='cap-right'/>
                      </div>
                    </div>
                    <div class='fauxcolumn-outer fauxcolumn-right-outer'>
                      <div class='cap-top'>
                        <div class='cap-left'/>
                        <div class='cap-right'/>
                      </div>
                      <div class='fauxborder-left'>
                        <div class='fauxborder-right'/>
                        <div class='fauxcolumn-inner'>
                        </div>
                      </div>
                      <div class='cap-bottom'>
                        <div class='cap-left'/>
                        <div class='cap-right'/>
                      </div>
                    </div>
                    <!-- corrects IE6 width calculation -->
                    <div class='columns-inner'>
                      <div class='column-center-outer'>
                        <div class='column-center-inner'>
                          <b:section class='main' id='main' name='Main' showaddelement='no'>
                            <b:widget id='Blog1' locked='false' title='Postingan Blog' type='Blog' version='1'>
                              <b:widget-settings>
                                <b:widget-setting name='showDateHeader'>true</b:widget-setting>
                                <b:widget-setting name='style.textcolor'>#ffffff</b:widget-setting>
                                <b:widget-setting name='showShareButtons'>true</b:widget-setting>
                                <b:widget-setting name='authorLabel'>By</b:widget-setting>
                                <b:widget-setting name='showCommentLink'>true</b:widget-setting>
                                <b:widget-setting name='style.urlcolor'>#ffffff</b:widget-setting>
                                <b:widget-setting name='showAuthor'>false</b:widget-setting>
                                <b:widget-setting name='style.linkcolor'>#ffffff</b:widget-setting>
                                <b:widget-setting name='style.unittype'>TextAndImage</b:widget-setting>
                                <b:widget-setting name='style.bgcolor'>#ffffff</b:widget-setting>
                                <b:widget-setting name='reactionsLabel'/>
                                <b:widget-setting name='showAuthorProfile'>false</b:widget-setting>
                                <b:widget-setting name='style.layout'>1x1</b:widget-setting>
                                <b:widget-setting name='showLabels'>true</b:widget-setting>
                                <b:widget-setting name='showLocation'>true</b:widget-setting>
                                <b:widget-setting name='showTimestamp'>true</b:widget-setting>
                                <b:widget-setting name='postsPerAd'>1</b:widget-setting>
                                <b:widget-setting name='showBacklinks'>false</b:widget-setting>
                                <b:widget-setting name='style.bordercolor'>#ffffff</b:widget-setting>
                                <b:widget-setting name='showInlineAds'>false</b:widget-setting>
                                <b:widget-setting name='showReactions'>false</b:widget-setting>
                              </b:widget-settings>
                              <b:includable id='main' var='top'>
                                <b:if cond='!data:mobile'>
                                  <!-- posts -->
                                  <div class='blog-posts hfeed'>
                                    <!--breadcrumbs start-->
                                    <b:if cond='data:blog.pageType == &quot;item&quot;'>
                                    <div class='breadcrumbs'>
                                           <div class='row'>
                                            <span class='post-labels'>
                                            <a expr:href='data:blog.homepageUrl' rel='tag'>Home</a>
                                            <b:loop values='data:posts' var='post'>
                                                <b:if cond='data:post.labels'>
                                                <b:loop values='data:post.labels' var='label'>
                                                    <b:if cond='data:label.isLast == true'> &#187;
                                                        <a expr:href='data:label.url + &quot;?&amp;max-results=10&quot;' rel='tag'><data:label.name/></a>
                                                    </b:if>
                                                </b:loop>
                                                <b:else/>
                                                &#187; Unlabelled
                                                </b:if>
                                                &#187; <span><data:post.title/></span>
                                            </b:loop>
                                            </span>
                                            </div>
                                        </div>
                                    </b:if>

                                    <b:if cond='data:blog.pageType == &quot;static_page&quot;'>
                                    <div class='breadcrumbs'>
                                     <div class='row'>
                                      <a expr:href='data:blog.homepageUrl'>Home</a> &#187; <data:blog.pageName/>
                                      </div>
                                    </div>
                                    </b:if>
                                    <b:if cond='data:blog.pageType == &quot;archive&quot;'>
                                        <div class='breadcrumbs'>
                                         <div class='row'>
                                          <a expr:href='data:blog.homepageUrl'>Home</a> &#187; <data:blog.pageName/>
                                          </div>
                                        </div>
                                    </b:if>
                                    <b:if cond='data:blog.searchLabel'>
                                        <div class='breadcrumbs'>
                                         <div class='row'>
                                          <a expr:href='data:blog.homepageUrl'>Home</a> &#187; <data:blog.pageName/>
                                          </div>
                                        </div>
                                    </b:if>
                                    <!--breadcrumbs end-->
                                    <b:include data='top' name='status-message'/>
                                    <b:loop values='data:posts' var='post'>
                                      <b:if cond='data:post.isDateStart and not data:post.isFirstPost'>
                                        &lt;/div&gt;&lt;/div&gt;
                                      </b:if>
                                      <b:if cond='data:post.isDateStart'>
                                        &lt;div class=&quot;date-outer&quot;&gt;
                                      </b:if>
                                      <b:if cond='data:post.isDateStart'>
                                        &lt;div class=&quot;date-posts&quot;&gt;
                                      </b:if>
                                      <div class='post-outer box-konten'>
                                        <b:include data='post' name='post'/>
                                        <b:include cond='data:blog.pageType in {&quot;static_page&quot;,&quot;item&quot;}' data='post' name='comment_picker'/>
                                      </div>
                                      <!-- Ad -->
                                      <b:if cond='data:post.includeAd'>
                                        <div class='inline-ad'>
                                          <data:adCode/>
                                        </div>
                                      </b:if>
                                    </b:loop>
                                    <b:if cond='data:numPosts != 0'>
                                      &lt;/div&gt;&lt;/div&gt;
                                    </b:if>
                                  </div>
                                  <!-- navigation -->
                                  <b:include name='nextprev'/>
                                  <!-- feed links -->
                                  <b:include name='feedLinks'/>
                                  <b:else/>
                                  <b:include name='mobile-main'/>
                                </b:if>
                                <b:if cond='data:top.showPlusOne'>
                                  <data:top.googlePlusBootstrap/>
                                </b:if>
                              </b:includable>
                              <b:includable id='backlinkDeleteIcon' var='backlink'>
                                <span expr:class='&quot;item-control &quot; + data:backlink.adminClass'>
                                  <a expr:href='data:backlink.deleteUrl' expr:title='data:top.deleteBacklinkMsg'>
                                    <img alt='backlink' src='https://resources.blogblog.com/img/icon_delete13.gif'/>
                                  </a>
                                </span>
                              </b:includable>
                              <b:includable id='backlinks' var='post'>
                                <a name='links'/>
                                <h4>
                                  <data:post.backlinksLabel/>
                                </h4>
                                <b:if cond='data:post.numBacklinks != 0'>
                                  <dl class='comments-block' id='comments-block'>
                                    <b:loop values='data:post.backlinks' var='backlink'>
                                      <div class='collapsed-backlink backlink-control'>
                                        <dt class='comment-title'>
                                          <span class='backlink-toggle-zippy'>
                                            &#160;
                                          </span>
                                          <a expr:href='data:backlink.url' rel='nofollow'>
                                            <data:backlink.title/>
                                          </a>
                                          <b:include data='backlink' name='backlinkDeleteIcon'/>
                                        </dt>
                                        <dd class='comment-body collapseable'>
                                          <data:backlink.snippet/>
                                        </dd>
                                        <dd class='comment-footer collapseable'>
                                          <span class='comment-author'>
                                            <data:post.authorLabel/>
                                            <data:backlink.author/>
                                          </span>
                                          <span class='comment-timestamp'>
                                            <data:post.timestampLabel/>
                                            <data:backlink.timestamp/>
                                          </span>
                                        </dd>
                                      </div>
                                    </b:loop>
                                  </dl>
                                </b:if>
                                <p class='comment-footer'>
                                  <a class='comment-link' expr:href='data:post.createLinkUrl' expr:id='data:widget.instanceId + &quot;_backlinks-create-link&quot;' target='_blank'>
                                    <data:post.createLinkLabel/>
                                  </a>
                                </p>
                              </b:includable>
                              <b:includable id='comment-form' var='post'>
                                <div class='comment-form'>
                                  <a name='comment-form'/>
                                  <b:if cond='data:mobile'>
                                    <h4 id='comment-post-message'>
                                      <a expr:id='data:widget.instanceId + &quot;_comment-editor-toggle-link&quot;' href='javascript:void(0)'>
                                        <data:postCommentMsg/>
                                      </a>
                                    </h4>
                                    <p>
                                      <data:blogCommentMessage/>
                                    </p>
                                    <data:blogTeamBlogMessage/>
                                    <a expr:href='data:post.commentFormIframeSrc' id='comment-editor-src'/>
                                    <iframe allowtransparency='true' class='blogger-iframe-colorize blogger-comment-from-post' expr:height='data:cmtIframeInitialHeight' frameborder='0' id='comment-editor' name='comment-editor' src='' style='display: none' width='100%'/>
                                    <b:else/>
                                    <h4 id='comment-post-message'>
                                      <data:postCommentMsg/>
                                    </h4>
                                    <p>
                                      <data:blogCommentMessage/>
                                    </p>
                                    <data:blogTeamBlogMessage/>
                                    <a expr:href='data:post.commentFormIframeSrc' id='comment-editor-src'/>
                                    <iframe allowtransparency='true' class='blogger-iframe-colorize blogger-comment-from-post' expr:height='data:cmtIframeInitialHeight' frameborder='0' id='comment-editor' name='comment-editor' src='' width='100%'/>
                                  </b:if>
                                  <data:post.cmtfpIframe/>
                                  <script type='text/javascript'>
                                    BLOG_CMT_createIframe(&#39;<data:post.appRpcRelayPath/>&#39;);
                                  </script>
                                </div>
                              </b:includable>
                              <b:includable id='commentDeleteIcon' var='comment'>
                                <span expr:class='&quot;item-control &quot; + data:comment.adminClass'>
                                  <b:if cond='data:showCmtPopup'>
                                    <div class='goog-toggle-button'>
                                      <div class='goog-inline-block comment-action-icon'/>
                                    </div>
                                    <b:else/>
                                    <a class='comment-delete' expr:href='data:comment.deleteUrl' expr:title='data:top.deleteCommentMsg'>
                                      <img alt='delete' src='https://resources.blogblog.com/img/icon_delete13.gif'/>
                                    </a>
                                  </b:if>
                                </span>
                              </b:includable>
                              <b:includable id='comment_count_picker' var='post'>
                                <b:if cond='data:post.commentSource == 1'>
                                  <span class='cmt_count_iframe_holder' expr:data-count='data:post.numComments' expr:data-onclick='data:post.addCommentOnclick' expr:data-post-url='data:post.url' expr:data-url='data:post.url.canonical.http'>
                                  </span>
                                  <b:else/>
                                  <a class='comment-link' expr:href='data:post.addCommentUrl' expr:onclick='data:post.addCommentOnclick'>
                                    <data:post.commentLabelFull/>
                                    :
                                  </a>
                                </b:if>
                              </b:includable>
                              <b:includable id='comment_picker' var='post'>
                                <b:if cond='data:post.commentSource == 1'>
                                  <b:include data='post' name='iframe_comments'/>
                                  <b:elseif cond='data:post.showThreadedComments'/>
                                  <b:include data='post' name='threaded_comments'/>
                                  <b:else/>
                                  <b:include data='post' name='comments'/>
                                </b:if>
                              </b:includable>
                              <b:includable id='comments' var='post'>
                               <div class='row'>
                                <div class='comments' id='comments'>
                                  <a name='comments'/>
                                  <b:if cond='data:post.allowComments'>
                                    <h4>
                                      <data:post.commentLabelFull/>
                                      :
                                    </h4>
                                    <b:if cond='data:post.commentPagingRequired'>
                                      <span class='paging-control-container'>
                                        <b:if cond='data:post.hasOlderLinks'>
                                          <a expr:class='data:post.oldLinkClass' expr:href='data:post.oldestLinkUrl'>
                                            <data:post.oldestLinkText/>
                                          </a>
                                          &#160;
                                          <a expr:class='data:post.oldLinkClass' expr:href='data:post.olderLinkUrl'>
                                            <data:post.olderLinkText/>
                                          </a>
                                          &#160;
                                        </b:if>
                                        <data:post.commentRangeText/>
                                        <b:if cond='data:post.hasNewerLinks'>
                                          &#160;
                                          <a expr:class='data:post.newLinkClass' expr:href='data:post.newerLinkUrl'>
                                            <data:post.newerLinkText/>
                                          </a>
                                          &#160;
                                          <a expr:class='data:post.newLinkClass' expr:href='data:post.newestLinkUrl'>
                                            <data:post.newestLinkText/>
                                          </a>
                                        </b:if>
                                      </span>
                                    </b:if>
                                    <div expr:id='data:widget.instanceId + &quot;_comments-block-wrapper&quot;'>
                                      <dl expr:class='data:post.avatarIndentClass' id='comments-block'>
                                        <b:loop values='data:post.comments' var='comment'>
                                          <dt expr:class='&quot;comment-author &quot; + data:comment.authorClass' expr:id='data:comment.anchorName'>
                                            <b:if cond='data:comment.favicon'>
                                              <img alt='favicon' expr:src='data:comment.favicon' height='16px' style='margin-bottom:-2px;' width='16px'/>
                                            </b:if>
                                            <a expr:name='data:comment.anchorName'/>
                                            <b:if cond='data:blog.enabledCommentProfileImages'>
                                              <data:comment.authorAvatarImage/>
                                            </b:if>
                                            <b:if cond='data:comment.authorUrl'>
                                              <a expr:href='data:comment.authorUrl' rel='nofollow'>
                                                <data:comment.author/>
                                              </a>
                                              <b:else/>
                                              <data:comment.author/>
                                            </b:if>
                                            <data:commentPostedByMsg/>
                                          </dt>
                                          <dd class='comment-body' expr:id='data:widget.instanceId + data:comment.cmtBodyIdPostfix'>
                                            <b:if cond='data:comment.isDeleted'>
                                              <span class='deleted-comment'>
                                                <data:comment.body/>
                                              </span>
                                              <b:else/>
                                              <p>
                                                <data:comment.body/>
                                              </p>
                                            </b:if>
                                          </dd>
                                          <dd class='comment-footer'>
                                            <span class='comment-timestamp'>
                                              <a expr:href='data:comment.url' title='comment permalink'>
                                                <data:comment.timestamp/>
                                              </a>
                                              <b:include data='comment' name='commentDeleteIcon'/>
                                            </span>
                                          </dd>
                                        </b:loop>
                                      </dl>
                                    </div>
                                    <b:if cond='data:post.commentPagingRequired'>
                                      <span class='paging-control-container'>
                                        <a expr:class='data:post.oldLinkClass' expr:href='data:post.oldestLinkUrl'>
                                          <data:post.oldestLinkText/>
                                        </a>
                                        <a expr:class='data:post.oldLinkClass' expr:href='data:post.olderLinkUrl'>
                                          <data:post.olderLinkText/>
                                        </a>
                                        &#160;
                                        <data:post.commentRangeText/>
                                        &#160;
                                        <a expr:class='data:post.newLinkClass' expr:href='data:post.newerLinkUrl'>
                                          <data:post.newerLinkText/>
                                        </a>
                                        <a expr:class='data:post.newLinkClass' expr:href='data:post.newestLinkUrl'>
                                          <data:post.newestLinkText/>
                                        </a>
                                      </span>
                                    </b:if>
                                    <p class='comment-footer'>
                                      <b:if cond='data:post.embedCommentForm'>
                                        <b:if cond='data:post.allowNewComments'>
                                          <b:include data='post' name='comment-form'/>
                                          <b:else/>
                                          <data:post.noNewCommentsText/>
                                        </b:if>
                                        <b:elseif cond='data:post.allowComments'/>
                                        <a expr:href='data:post.addCommentUrl' expr:onclick='data:post.addCommentOnclick'>
                                          <data:postCommentMsg/>
                                        </a>
                                      </b:if>
                                    </p>
                                  </b:if>
                                  <b:if cond='data:showCmtPopup'>
                                    <div id='comment-popup'>
                                      <iframe allowtransparency='true' frameborder='0' id='comment-actions' name='comment-actions' scrolling='no'>
                                      </iframe>
                                    </div>
                                  </b:if>
                                  <div id='backlinks-container'>
                                    <div expr:id='data:widget.instanceId + &quot;_backlinks-container&quot;'>
                                      <b:include cond='data:post.showBacklinks' data='post' name='backlinks'/>
                                    </div>
                                  </div>
                                </div>
                                </div>
                              </b:includable>
                              <b:includable id='feedLinks'>
                                <b:if cond='data:blog.pageType != &quot;item&quot;'>
                                  <!-- Blog feed links -->
                                  <b:if cond='data:feedLinks'>
                                    <div class='blog-feeds'>
                                      <b:include data='feedLinks' name='feedLinksBody'/>
                                    </div>
                                  </b:if>
                                  <b:else/>
                                  <!--Post feed links -->
                                  <div class='post-feeds'>
                                    <b:loop values='data:posts' var='post'>
                                      <b:include cond='data:post.allowComments and data:post.feedLinks' data='post.feedLinks' name='feedLinksBody'/>
                                    </b:loop>
                                  </div>
                                </b:if>
                              </b:includable>
                              <b:includable id='feedLinksBody' var='links'>
                              </b:includable>
                              <b:includable id='iframe_comments' var='post'>
                                <b:if cond='data:post.allowIframeComments'>
                                  <script expr:src='data:post.iframeCommentSrc' type='text/javascript'/>
                                  <div class='cmt_iframe_holder' expr:data-href='data:post.url.canonical' expr:data-viewtype='data:post.viewType'/>
                                  <b:if cond='data:post.embedCommentForm == &quot;false&quot;'>
                                    <a expr:href='data:post.addCommentUrl' expr:onclick='data:post.addCommentOnclick'>
                                      <data:postCommentMsg/>
                                    </a>
                                  </b:if>
                                </b:if>
                              </b:includable>
                              <b:includable id='mobile-index-post' var='post'>
                                <div class='mobile-date-outer date-outer'>
                                  <b:if cond='data:post.dateHeader'>
                                    <div class='date-header'>
                                      <span>
                                        <data:post.dateHeader/>
                                      </span>
                                    </div>
                                  </b:if>
                                  <div class='mobile-post-outer'>
                                    <a expr:href='data:post.url'>
                                      <h3 class='mobile-index-title entry-title' itemprop='name'>
                                        <data:post.title/>
                                      </h3>
                                      <div class='mobile-index-arrow'>
                                        &amp;rsaquo;
                                      </div>
                                      <div class='mobile-index-contents'>
                                        <b:if cond='data:post.thumbnailUrl'>
                                          <div class='mobile-index-thumbnail'>
                                            <div class='Image'>
                                              <img expr:src='data:post.thumbnailUrl'/>
                                            </div>
                                          </div>
                                        </b:if>
                                        <div class='post-body'>
                                          <b:if cond='data:post.snippet'>
                                            <data:post.snippet/>
                                          </b:if>
                                        </div>
                                      </div>
                                      <div style='clear: both;'/>
                                    </a>
                                    <div class='mobile-index-comment'>
                                      <b:include cond='data:blog.pageType != &quot;static_page&quot;                          and data:post.allowComments                          and data:post.numComments != 0' data='post' name='comment_count_picker'/>
                                    </div>
                                  </div>
                                </div>
                              </b:includable>
                              <b:includable id='mobile-main' var='top'>
                                <!-- posts -->
                                <div class='blog-posts hfeed'>
                                  <b:include data='top' name='status-message'/>
                                  <b:if cond='data:blog.pageType == &quot;index&quot;'>
                                    <b:loop values='data:posts' var='post'>
                                      <b:include data='post' name='mobile-index-post'/>
                                    </b:loop>
                                    <b:else/>
                                    <b:loop values='data:posts' var='post'>
                                      <b:include data='post' name='mobile-post'/>
                                    </b:loop>
                                  </b:if>
                                </div>
                                <b:include name='mobile-nextprev'/>
                              </b:includable>
                              <b:includable id='mobile-nextprev'>
                                <div class='blog-pager' id='blog-pager'>
                                  <b:if cond='data:newerPageUrl'>
                                    <div class='mobile-link-button' id='blog-pager-newer-link'>
                                      <a class='blog-pager-newer-link' expr:href='data:newerPageUrl' expr:id='data:widget.instanceId + &quot;_blog-pager-newer-link&quot;' expr:title='data:newerPageTitle'>
                                        &amp;lsaquo;
                                      </a>
                                    </div>
                                  </b:if>
                                  <b:if cond='data:olderPageUrl'>
                                    <div class='mobile-link-button' id='blog-pager-older-link'>
                                      <a class='blog-pager-older-link' expr:href='data:olderPageUrl' expr:id='data:widget.instanceId + &quot;_blog-pager-older-link&quot;' expr:title='data:olderPageTitle'>
                                        &amp;rsaquo;
                                      </a>
                                    </div>
                                  </b:if>
                                  <div class='mobile-link-button' id='blog-pager-home-link'>
                                    <a class='home-link' expr:href='data:blog.homepageUrl'>
                                      <data:homeMsg/>
                                    </a>
                                  </div>
                                  <div class='mobile-desktop-link'>
                                    <a class='home-link' expr:href='data:desktopLinkUrl'>
                                      <data:desktopLinkMsg/>
                                    </a>
                                  </div>
                                </div>
                                <div class='clear'/>
                              </b:includable>
                              <b:includable id='mobile-post' var='post'>
                                <div class='date-outer'>
                                  <b:if cond='data:post.dateHeader'>
                                    <h2 class='date-header'>
                                      <span>
                                        <data:post.dateHeader/>
                                      </span>
                                    </h2>
                                  </b:if>
                                  <div class='date-posts'>
                                    <div class='post-outer box-konten'>
                                     <!--div class='row'-->
                                     <div class='row'>
                                      <div class='post hentry uncustomized-post-template' itemscope='itemscope' itemtype='http://schema.org/BlogPosting'>
                                        <b:if cond='data:post.thumbnailUrl'>
                                          <meta expr:content='data:post.thumbnailUrl' itemprop='image_url'/>
                                        </b:if>
                                        <meta expr:content='data:blog.blogId' itemprop='blogId'/>
                                        <meta expr:content='data:post.id' itemprop='postId'/>
                                        <a expr:name='data:post.id'/>
                                        <b:if cond='data:post.title'>
                                          <h2 class='post-title entry-title' itemprop='name'>
                                            <b:if cond='data:post.link'>
                                              <a expr:href='data:post.link'>
                                                <data:post.title/>
                                              </a>
                                              <b:elseif cond='data:post.url and data:blog.url != data:post.url'/>
                                              <a expr:href='data:post.url'>
                                                <data:post.title/>
                                              </a>
                                              <b:else/>
                                              <data:post.title/>
                                            </b:if>
                                          </h2>
                                        </b:if>
                                        <div class='row'>
                                        <div class='post-header'>
                                          <div class='post-header-line-1'/>

                                        </div>
                                        </div>
                                        <div class='post-body entry-content' expr:id='&quot;post-body-&quot; + data:post.id' itemprop='articleBody'>
                                          <data:post.body/>
                                          <div style='clear: both;'/>
                                          <!-- clear for photos floats -->
                                        </div>
                                        <div class='row'>
                                        <div class='post-footer'>
                                          <div class='post-footer-line post-footer-line-1'>
                                            <span class='post-author vcard'>
                                              <b:if cond='data:top.showAuthor'>
                                                <b:if cond='data:post.authorProfileUrl'>
                                                  <span class='fn' itemprop='author' itemscope='itemscope' itemtype='http://schema.org/Person'>
                                                    <meta expr:content='data:post.authorProfileUrl' itemprop='url'/>
                                                    <a expr:href='data:post.authorProfileUrl' rel='author' title='author profile'>
                                                      <span itemprop='name'>
                                                        <data:post.author/>
                                                      </span>
                                                    </a>
                                                  </span>
                                                  <b:else/>
                                                  <span class='fn' itemprop='author' itemscope='itemscope' itemtype='http://schema.org/Person'>
                                                    <span itemprop='name'>
                                                      <data:post.author/>
                                                    </span>
                                                  </span>
                                                </b:if>
                                              </b:if>
                                            </span>
                                            <span class='post-timestamp'>
                                              <b:if cond='data:top.showTimestamp'>
                                                <data:top.timestampLabel/>
                                                <b:if cond='data:post.url'>
                                                  <meta expr:content='data:post.url.canonical' itemprop='url'/>
                                                  <a class='timestamp-link' expr:href='data:post.url' rel='bookmark' title='permanent link'>
                                                    <abbr class='published' expr:title='data:post.timestampISO8601' itemprop='datePublished'>
                                                      <data:post.timestamp/>
                                                    </abbr>
                                                  </a>
                                                </b:if>
                                              </b:if>
                                            </span>
                                            <span class='post-comment-link'>
                                              <b:include cond='data:blog.pageType not in {&quot;item&quot;,&quot;static_page&quot;}                                  and data:post.allowComments' data='post' name='comment_count_picker'/>
                                            </span>
                                          </div>
                                          <div class='post-footer-line post-footer-line-2'>
                                            <b:if cond='data:top.showMobileShare'>
                                              <div class='mobile-link-button goog-inline-block' id='mobile-share-button'>
                                                <a href='javascript:void(0);'>
                                                  <data:shareMsg/>
                                                </a>
                                              </div>
                                            </b:if>
                                            <b:if cond='data:top.showDummy'>
                                              <div class='goog-inline-block dummy-container'>
                                                <data:post.dummyTag/>
                                              </div>
                                            </b:if>
                                          </div>
                                        </div>
                                        </div>
                                      </div>
                                      <b:include cond='data:blog.pageType in {&quot;static_page&quot;,&quot;item&quot;}' data='post' name='comment_picker'/>
                                        </div>
                                      <!--/div row-->
                                    </div>
                                  </div>
                                </div>
                              </b:includable>
                              <b:includable id='nextprev'>
                                <b:if cond='data:blog.pageType != &quot;item&quot;'>
                                <b:if cond='data:blog.pageType != &quot;static_page&quot;'>
                                  <div class='blog-pager' id='blog-pager'>
                                    <b:if cond='data:newerPageUrl'>
                                      <span id='blog-pager-newer-link'>
                                      <a class='blog-pager-newer-link' expr:href='data:newerPageUrl' expr:id='data:widget.instanceId + &quot;_blog-pager-newer-link&quot;' expr:title='data:newerPageTitle'><data:newerPageTitle/></a>
                                      </span>
                                    </b:if>
                                    <b:if cond='data:olderPageUrl'>
                                      <span id='blog-pager-older-link'>
                                      <a class='blog-pager-older-link' expr:href='data:olderPageUrl' expr:id='data:widget.instanceId + &quot;_blog-pager-older-link&quot;' expr:title='data:olderPageTitle'><data:olderPageTitle/></a>
                                      </span>
                                    </b:if>
                                    <a class='home-link' expr:href='data:blog.homepageUrl'><data:homeMsg/></a>
                                    <b:if cond='data:mobileLinkUrl'>
                                      <div class='blog-mobile-link'>
                                        <a expr:href='data:mobileLinkUrl'><data:mobileLinkMsg/></a>
                                      </div>
                                    </b:if>
                                </div>
                                </b:if></b:if>
                                <div class='clear'/>
                              </b:includable>
                              <b:includable id='post' var='post'>
                                <div class='post hentry uncustomized-post-template' itemprop='blogPost' itemscope='itemscope' itemtype='http://schema.org/BlogPosting'>
                                  <b:if cond='data:post.firstImageUrl'>
                                    <meta expr:content='data:post.firstImageUrl' itemprop='image_url'/>
                                  </b:if>
                                  <meta expr:content='data:blog.blogId' itemprop='blogId'/>
                                  <meta expr:content='data:post.id' itemprop='postId'/>
                                  <a expr:name='data:post.id'/>
                                  <b:if cond='data:post.title'>
                                    <div class='row'>
                                    <h2 class='post-title entry-title' itemprop='name'>
                                      <b:if cond='data:post.link or (data:post.url and data:blog.url != data:post.url)'>
                                        <a expr:href='data:post.link ? data:post.link : data:post.url'>
                                          <data:post.title/>
                                        </a>
                                        <b:else/>
                                        <data:post.title/>
                                      </b:if>
                                    </h2>
                                    </div>
                                  </b:if>
                                  <div class='row'>
                                  <div class='post-header'>
                                    <div class='post-header-line-1'/>
                                    <!-- meta dibawah judul (detail) -->
                                    <span class='post-author vcard'>
                                        <b:if cond='data:top.showAuthor'>
                                          <data:top.authorLabel/>
                                          <b:if cond='data:post.authorProfileUrl'>
                                            <span class='fn' itemprop='author' itemscope='itemscope' itemtype='http://schema.org/Person'>
                                              <meta expr:content='data:post.authorProfileUrl' itemprop='url'/>
                                              <a class='g-profile' expr:href='data:post.authorProfileUrl' rel='author' title='author profile'>
                                                <span itemprop='name'>
                                                  <data:post.author/>
                                                </span>
                                              </a>
                                            </span>
                                            <b:else/>
                                            <span class='fn' itemprop='author' itemscope='itemscope' itemtype='http://schema.org/Person'>
                                              <span itemprop='name'>
                                                <data:post.author/>
                                              </span>
                                            </span>
                                          </b:if>
                                        </b:if>
                                      </span>
                                      <span class='post-timestamp'>
                                        <b:if cond='data:top.showTimestamp'>
                                          <data:top.timestampLabel/>
                                          <b:if cond='data:post.url'>
                                            <meta expr:content='data:post.url.canonical' itemprop='url'/>
                                            <a class='timestamp-link' expr:href='data:post.url' rel='bookmark' title='permanent link'>
                                              <abbr class='published' expr:title='data:post.timestampISO8601' itemprop='datePublished'>
                                                <data:post.timestamp/>
                                              </abbr>
                                            </a>
                                          </b:if>
                                        </b:if>
                                      </span>
                                  </div>
                                  </div>
                                  <!-- Then use the post body as the schema.org description, for good G+/FB snippeting. -->
                                  <div class='post-body entry-content' expr:id='&quot;post-body-&quot; + data:post.id' expr:itemprop='(data:blog.metaDescription ? &quot;&quot; : &quot;description &quot;) + &quot;articleBody&quot;'>
                                    <!--data:post.body/  katanya disuruh ganti -->
                                    <b:if cond='data:blog.pageType == &quot;static_page&quot;'>
                                      <data:post.body/>
                                      <b:else/>
                                      <b:if cond='data:blog.pageType != &quot;item&quot;'>
                                        <div class='row' expr:id='&quot;summary&quot; + data:post.id'>
                                          <data:post.body/>
                                        </div>
                                        <script type='text/javascript'>
                                          createSummaryAndThumb(&quot;summary<data:post.id/>&quot;);
                                        </script>

                                      </b:if>
                                      <b:if cond='data:blog.pageType == &quot;item&quot;'>
                                        <data:post.body/>
                                      </b:if>
                                    </b:if>
                                    <!-- selesai diganti -->
                                    <div style='clear: both;'/>
                                    <!-- clear for photos floats -->
                                  </div>
                                  <!--b:if cond='data:post.hasJumpLink'>
                                    <div class='jump-link'>
                                      <a expr:href='data:post.url + &quot;#more&quot;' expr:title='data:post.title'>
                                        <data:post.jumpText/>
                                      </a>
                                    </div>
                                  </b:if-->
                                  <div class='row'>
                                  <div class='post-footer'>
                                    <div class='post-footer-line post-footer-line-1'/>
                                    <div class='post-footer-line post-footer-line-2'>
                                     <b:if cond='data:blog.pageType == &quot;item&quot;'>
                                      <span class='post-labels'>
                                        <b:if cond='data:top.showPostLabels and data:post.labels'>
                                          Tags :
                                          <b:loop values='data:post.labels' var='label'>
                                            <a expr:href='data:label.url + &quot;?&amp;max-results=10&quot;' rel='tag'>
                                              <data:label.name/>
                                            </a>
                                            <b:if cond='not data:label.isLast'>
                                              ,
                                            </b:if>
                                          </b:loop>
                                        </b:if>
                                      </span>
                                        </b:if>
                                    </div>
                                    <div class='post-footer-line post-footer-line-3'>
                                        <b:if cond='data:blog.pageType == &quot;item&quot;'>
                                          <div class='bagikan'>

                                          <div class='label-bagikan'>
                                            <strong>BAGIKAN </strong>
                                          </div>

                                          <a class='facebook' expr:href='&quot;http://www.facebook.com/sharer.php?u=&quot; + data:post.url + &quot;&amp;title=&quot;+ data:post.title' onclick='window.open(this.href, &apos;windowName&apos;, &apos;width=600, height=400, left=24, top=24, scrollbars, resizable&apos;); return false;' rel='nofollow' target='_blank'><i class='fa fa-facebook'/><span> Share </span></a>

                                          <a class='twitter' expr:href='&quot;http://twitter.com/share?url=&quot; + data:post.url + &quot;&amp;title=&quot; + data:post.title' onclick='window.open(this.href, &apos;windowName&apos;, &apos;width=600, height=400, left=24, top=24, scrollbars, resizable&apos;); return false;' rel='nofollow' target='_blank'><i class='fa fa-twitter'/><span> Tweet </span></a>

                                          <a class='googleplus' expr:href='&quot;https://plus.google.com/share?url=&quot; + data:post.url + &quot;&amp;title=&quot; + data:post.title' onclick='window.open(this.href, &apos;windowName&apos;, &apos;width=600, height=400, left=24, top=24, scrollbars, resizable&apos;); return false;' rel='nofollow' target='_blank'><i class='fa fa-google-plus'/><span> Share </span></a>

                                          <a class='linkedin' expr:href='&quot;http://www.linkedin.com/shareArticle?url=&quot; + data:post.url + &quot;&amp;title=&quot;+ data:post.title' onclick='window.open(this.href, &apos;windowName&apos;, &apos;width=600, height=400, left=24, top=24, scrollbars, resizable&apos;); return false;' rel='nofollow' target='_blank'><i class='fa fa-linkedin'/><span> Share </span></a>

                                          <a class='pinterest' expr:href='&quot;http://pinterest.com/pin/create/button/?url=&quot; + data:post.url + &quot;&amp;media=&quot; + data:post.firstImageUrl + &quot;&amp;description=&quot; + data:post.snippet' onclick='window.open(this.href, &apos;windowName&apos;, &apos;width=600, height=400, left=24, top=24, scrollbars, resizable&apos;); return false;' rel='nofollow' target='_blank'><i class='fa fa-pinterest-p'/><span> Pin </span></a>

                                          <a class='whatsapp' expr:href='&quot;https://api.whatsapp.com/send?text=&quot; + data:post.url + &quot;&amp;title=&quot;+ data:post.title' onclick='window.open(this.href, &apos;windowName&apos;, &apos;width=600, height=400, left=24, top=24, scrollbars, resizable&apos;); return false;' rel='nofollow' target='_blank'><i class='fa fa-whatsapp'/><span> Share </span></a>


                                        </div>
                                        </b:if>
                                    </div>

                                    <b:if cond='data:blog.pageType == &quot;item&quot;'>
                                        <div class='blog-pager' id='blog-pager'>
                                            <div class='pager-content'>
                                                <div id='blog-pager-newer-link'>
                                                   <b:if cond='data:olderPageUrl'>
                                                      <a class='blog-pager-older-link' expr:href='data:olderPageUrl' expr:id='data:widget.instanceId + &quot;_blog-pager-older-link&quot;' expr:title='data:olderPageTitle'>
                                                          <h6> Prev</h6>

                                                        <data:olderPageTitle/>
                                                      </a>
                                                    </b:if>

                                                </div>
                                                <div id='blog-pager-older-link'>
                                                    <b:if cond='data:newerPageUrl'>
                                                      <a class='blog-pager-newer-link' expr:href='data:newerPageUrl' expr:id='data:widget.instanceId + &quot;_blog-pager-newer-link&quot;' expr:title='data:newerPageTitle'>
                                                          <h6>Next  </h6>

                                                        <data:newerPageTitle/>
                                                      </a>
                                                    </b:if>
                                                </div>
                                             </div>
                                            <div class='clear'/>
                                        </div>
                                        <script type='text/javascript'>
                                        //<![CDATA[
                                        (function($){
                                            var newerLink = $('a.blog-pager-newer-link');
                                            var olderLink = $('a.blog-pager-older-link');
                                            $.get(newerLink.attr('href'), function (data) {
                                             newerLink.html('<h6>Next <i class="fa fa-chevron-right"/></h6><span>'+$(data).find('.post h2.post-title').text()+'</span>');
                                            },"html");
                                            $.get(olderLink.attr('href'), function (data2) {
                                             olderLink.html('<h6><i class="fa fa-chevron-left"/> Prev</h6><span>'+$(data2).find('.post h2.post-title').text()+'</span>');
                                            },"html");
                                        })(jQuery);
                                        //]]>
                                        </script>
                                        </b:if>
                                  </div>
                                  </div>
                                  <!-- Related Posts with Thumbnails Code Start-->
                                <b:if cond='data:blog.pageType == &quot;item&quot;'>
                                <div class='row'>
                                    <div id='related-posts'>
                                    <b:loop values='data:post.labels' var='label'>
                                    <b:if cond='data:label.isLast != &quot;true&quot;'>
                                    </b:if>
                                    <script expr:src='&quot;/feeds/posts/default/-/&quot; + data:label.name + &quot;?alt=json-in-script&amp;callback=related_results_labels_thumbs&amp;max-results=6&quot;' type='text/javascript'/></b:loop>
                                    <script type='text/javascript'>
                                    var currentposturl=&quot;<data:post.url/>&quot;;
                                    var maxresults=6;
                                    var relatedpoststitle=&quot;<b>Related Posts:</b>&quot;;
                                    removeRelatedDuplicates_thumbs();
                                    printRelatedLabels_thumbs();
                                    </script>
                                    </div>
                                </div>
                                <div class='clear'/>
                                </b:if>
                                <!-- Related Posts with Thumbnails Code End-->
                                </div>
                              </b:includable>
                              <b:includable id='postQuickEdit' var='post'>
                                <b:if cond='data:post.editUrl'>
                                  <span expr:class='&quot;item-control &quot; + data:post.adminClass'>
                                    <a expr:href='data:post.editUrl' expr:title='data:top.editPostMsg'>
                                      <img alt='edit' class='icon-action' height='18' src='https://resources.blogblog.com/img/icon18_edit_allbkg.gif' width='18'/>
                                    </a>
                                  </span>
                                </b:if>
                              </b:includable>
                              <b:includable id='shareButtons' var='post'>
                                <b:if cond='data:top.showEmailButton'>
                                  <a class='goog-inline-block share-button sb-email' expr:href='data:post.sharePostUrl + &quot;&amp;target=email&quot;' expr:title='data:top.emailThisMsg' target='_blank'>
                                    <span class='share-button-link-text'>
                                      <data:top.emailThisMsg/>
                                    </span>
                                  </a>
                                </b:if>
                                <b:if cond='data:top.showBlogThisButton'>
                                  <a class='goog-inline-block share-button sb-blog' expr:href='data:post.sharePostUrl + &quot;&amp;target=blog&quot;' expr:onclick='&quot;window.open(this.href, \&quot;_blank\&quot;, \&quot;height=270,width=475\&quot;); return false;&quot;' expr:title='data:top.blogThisMsg' target='_blank'>
                                    <span class='share-button-link-text'>
                                      <data:top.blogThisMsg/>
                                    </span>
                                  </a>
                                </b:if>
                                <b:if cond='data:top.showTwitterButton'>
                                  <a class='goog-inline-block share-button sb-twitter' expr:href='data:post.sharePostUrl + &quot;&amp;target=twitter&quot;' expr:title='data:top.shareToTwitterMsg' target='_blank'>
                                    <span class='share-button-link-text'>
                                      <data:top.shareToTwitterMsg/>
                                    </span>
                                  </a>
                                </b:if>
                                <b:if cond='data:top.showFacebookButton'>
                                  <a class='goog-inline-block share-button sb-facebook' expr:href='data:post.sharePostUrl + &quot;&amp;target=facebook&quot;' expr:onclick='&quot;window.open(this.href, \&quot;_blank\&quot;, \&quot;height=430,width=640\&quot;); return false;&quot;' expr:title='data:top.shareToFacebookMsg' target='_blank'>
                                    <span class='share-button-link-text'>
                                      <data:top.shareToFacebookMsg/>
                                    </span>
                                  </a>
                                </b:if>
                                <b:if cond='data:top.showPinterestButton'>
                                  <a class='goog-inline-block share-button sb-pinterest' expr:href='data:post.sharePostUrl + &quot;&amp;target=pinterest&quot;' expr:title='data:top.shareToPinterestMsg' target='_blank'>
                                    <span class='share-button-link-text'>
                                      <data:top.shareToPinterestMsg/>
                                    </span>
                                  </a>
                                </b:if>
                                <b:if cond='data:top.showPlusOne'>
                                  <div class='goog-inline-block google-plus-share-container'>
                                    <data:post.googlePlusShareTag/>
                                  </div>
                                </b:if>
                              </b:includable>
                              <b:includable id='status-message'>
                                <b:if cond='data:navMessage'>
                                <div>
                                </div>
                                <div style='clear: both;'/>
                                </b:if>
                              </b:includable>
                              <b:includable id='threaded-comment-form' var='post'>
                                <div class='comment-form'>
                                  <a name='comment-form'/>
                                  <b:if cond='data:mobile'>
                                    <p>
                                      <data:blogCommentMessage/>
                                    </p>
                                    <data:blogTeamBlogMessage/>
                                    <a expr:href='data:post.commentFormIframeSrc' id='comment-editor-src'/>
                                    <iframe allowtransparency='true' class='blogger-iframe-colorize blogger-comment-from-post' expr:height='data:cmtIframeInitialHeight' frameborder='0' id='comment-editor' name='comment-editor' src='' style='display: none' width='100%'/>
                                    <b:else/>
                                    <p>
                                      <data:blogCommentMessage/>
                                    </p>
                                    <data:blogTeamBlogMessage/>
                                    <a expr:href='data:post.commentFormIframeSrc' id='comment-editor-src'/>
                                    <iframe allowtransparency='true' class='blogger-iframe-colorize blogger-comment-from-post' expr:height='data:cmtIframeInitialHeight' frameborder='0' id='comment-editor' name='comment-editor' src='' width='100%'/>
                                  </b:if>
                                  <data:post.cmtfpIframe/>
                                  <script type='text/javascript'>
                                    BLOG_CMT_createIframe(&#39;<data:post.appRpcRelayPath/>&#39;);
                                  </script>
                                </div>
                              </b:includable>
                              <b:includable id='threaded_comment_js' var='post'>
                                <script async='async' expr:src='data:post.commentSrc' type='text/javascript'/>
                                <script type='text/javascript'>
                                  (function() {
                                    var items = <data:post.commentJso/>;
                                    var msgs = <data:post.commentMsgs/>;
                                    var config = <data:post.commentConfig/>;
                                    // <![CDATA[
                                    var cursor=null;items&&items.length>0&&(cursor=parseInt(items[items.length-1].timestamp)+1);var bodyFromEntry=function(a){if(a.gd$extendedProperty)for(var b in a.gd$extendedProperty)if("blogger.contentRemoved"==a.gd$extendedProperty[b].name)return'<span class="deleted-comment">'+a.content.$t+"</span>";return a.content.$t},parse=function(a){cursor=null;var b=[];if(a&&a.feed&&a.feed.entry)for(var d,c=0;d=a.feed.entry[c];c++){var e={},f=/blog-(\d+).post-(\d+)/.exec(d.id.$t);if(e.id=f?f[2]:null,e.body=bodyFromEntry(d),e.timestamp=Date.parse(d.published.$t)+"",d.author&&d.author.constructor===Array){var g=d.author[0];g&&(e.author={name:g.name?g.name.$t:void 0,profileUrl:g.uri?g.uri.$t:void 0,avatarUrl:g.gd$image?g.gd$image.src:void 0})}if(d.link&&(d.link[2]&&(e.link=e.permalink=d.link[2].href),d.link[3])){var h=/.*comments\/default\/(\d+)\?.*/.exec(d.link[3].href);h&&h[1]&&(e.parentId=h[1])}if(e.deleteclass="item-control blog-admin",d.gd$extendedProperty)for(var i in d.gd$extendedProperty)"blogger.itemClass"==d.gd$extendedProperty[i].name?e.deleteclass+=" "+d.gd$extendedProperty[i].value:"blogger.displayTime"==d.gd$extendedProperty[i].name&&(e.displayTime=d.gd$extendedProperty[i].value);b.push(e)}return b},paginator=function(a){if(hasMore()){var b=config.feed+"?alt=json&v=2&orderby=published&reverse=false&max-results=50";cursor&&(b+="&published-min="+new Date(cursor).toISOString()),window.bloggercomments=function(b){var c=parse(b);cursor=c.length<50?null:parseInt(c[c.length-1].timestamp)+1,a(c),window.bloggercomments=null},b+="&callback=bloggercomments";var c=document.createElement("script");c.type="text/javascript",c.src=b,document.getElementsByTagName("head")[0].appendChild(c)}},hasMore=function(){return!!cursor},getMeta=function(a,b){if("iswriter"==a){var c=!!b.author&&b.author.name==config.authorName&&b.author.profileUrl==config.authorUrl;return c?"true":""}return"deletelink"==a?config.baseUri+"/delete-comment.g?blogID="+config.blogId+"&postID="+b.id:"deleteclass"==a?b.deleteclass:""},replybox=null,replyUrlParts=null,replyParent=void 0,onReply=function(a,b){null==replybox&&(replybox=document.getElementById("comment-editor"),null!=replybox&&(replybox.height="250px",replybox.style.display="block",replyUrlParts=replybox.src.split("#"))),replybox&&a!==replyParent&&(replybox.src="",document.getElementById(b).insertBefore(replybox,null),replybox.src=replyUrlParts[0]+(a?"&parentID="+a:"")+"#"+replyUrlParts[1],replyParent=a)},hash=(window.location.hash||"#").substring(1),startThread,targetComment;/^comment-form_/.test(hash)?startThread=hash.substring("comment-form_".length):/^c[0-9]+$/.test(hash)&&(targetComment=hash.substring(1));var configJso={maxDepth:config.maxThreadDepth},provider={id:config.postId,data:items,loadNext:paginator,hasMore:hasMore,getMeta:getMeta,onReply:onReply,rendered:!0,initComment:targetComment,initReplyThread:startThread,config:configJso,messages:msgs},render=function(){if(window.goog&&window.goog.comments){var a=document.getElementById("comment-holder");window.goog.comments.render(a,provider)}};window.goog&&window.goog.comments?render():(window.goog=window.goog||{},window.goog.comments=window.goog.comments||{},window.goog.comments.loadQueue=window.goog.comments.loadQueue||[],window.goog.comments.loadQueue.push(render));
                                  })();
                                  // ]]>
                                </script>
                              </b:includable>
                              <b:includable id='threaded_comments' var='post'>
                               <div class='row'>
                                <div class='comments' id='comments'>
                                  <a name='comments'/>
                                  <h4>
                                    <data:post.commentLabelFull/>
                                    :
                                  </h4>
                                  <div class='comments-content'>
                                    <b:include cond='data:post.embedCommentForm' data='post' name='threaded_comment_js'/>
                                    <div id='comment-holder'>
                                      <data:post.commentHtml/>
                                    </div>
                                  </div>
                                  <p class='comment-footer'>
                                    <b:if cond='data:post.allowNewComments'>
                                      <b:include data='post' name='threaded-comment-form'/>
                                      <b:else/>
                                      <data:post.noNewCommentsText/>
                                    </b:if>
                                  </p>
                                  <b:if cond='data:showCmtPopup'>
                                    <div id='comment-popup'>
                                      <iframe allowtransparency='true' frameborder='0' id='comment-actions' name='comment-actions' scrolling='no'>
                                      </iframe>
                                    </div>
                                  </b:if>
                                  <div id='backlinks-container'>
                                    <div expr:id='data:widget.instanceId + &quot;_backlinks-container&quot;'>
                                      <b:include cond='data:post.showBacklinks' data='post' name='backlinks'/>
                                    </div>
                                  </div>
                                </div>
                                </div>
                              </b:includable>
                            </b:widget>
                          </b:section>
                        </div>
                      </div>
                      <div class='column-left-outer'>
                        <div class='column-left-inner'>
                          <aside>
                            <macro:include id='main-column-left-sections' name='sections'>
                              <macro:param default='0' name='num' value='0'/>
                              <macro:param default='sidebar-left' name='idPrefix'/>
                              <macro:param default='sidebar' name='class'/>
                              <macro:param default='true' name='includeBottom'/>
                            </macro:include>
                          </aside>
                        </div>
                      </div>
                      <div class='column-right-outer'>
                        <div class='column-right-inner'>
                          <aside>
                            <macro:include id='main-column-right-sections' name='sections'>
                              <macro:param default='2' name='num' value='0'/>
                              <macro:param default='sidebar-right' name='idPrefix'/>
                              <macro:param default='sidebar' name='class'/>
                              <macro:param default='true' name='includeBottom'/>
                            </macro:include>
                          </aside>
                        </div>
                      </div>
                    </div>
                    <div style='clear: both'/>
                    <!-- columns -->
                  </div>
                  <!-- main -->
                </div>
              </div>
              <div class='main-cap-bottom cap-bottom'>
                <div class='cap-left'/>
                <div class='cap-right'/>
              </div>
            </div>

            <!-- content -->
          </div>
<!-- end content-inner -->

<footer class='footer-global'>
    <div class='footer-outer'>
    <div class='footer-cap-top cap-top'>
      <div class='cap-left'/>
      <div class='cap-right'/>
    </div>
    <div class='fauxborder-left footer-fauxborder-left'>
    <div class='fauxborder-right footer-fauxborder-right'/>
    <div class='region-inner footer-inner'>
      <macro:include id='footer-sections' name='sections'>
        <macro:param default='3' name='num'/>
        <macro:param default='footer' name='idPrefix'/>
        <macro:param default='foot' name='class'/>
        <macro:param default='false' name='includeBottom'/>
      </macro:include>
    </div>
    </div>
    <div class='footer-cap-bottom cap-bottom'>
      <div class='cap-left'/>
      <div class='cap-right'/>
    </div>
    </div>
    </footer>

    <footer class='copy'>
        <p>Copyright &#169; <a expr:href='data:blog.homepageUrl'><data:blog.title/></a>  <script>document.write(new Date().getFullYear())</script> | Desain oleh : <a href='http://themes.aroodam.com/landing-page'>Aroodam Landing Page</a> |  <a href='#atas'> top <i aria-hidden='true' class='fa fa-arrow-up'/></a></p>
    </footer>

        </div>
        <div class='content-cap-bottom cap-bottom'>
          <div class='cap-left'/>
          <div class='cap-right'/>
        </div>
      </div>
    </div>
    <script type='text/javascript'>
      window.setTimeout(function() {
        document.body.className = document.body.className.replace(&#39;loading&#39;, &#39;&#39;);}, 10);
    </script>

    <!--b:if cond='data:blog.pageType != &quot;item&quot;'>
    <b:if cond='data:blog.pageType != &quot;static_page&quot;'-->
    <script type='text/javascript'>
      /*<![CDATA[*/
        var perPage=3;
        var numPages=3;
        var firstText ='First';
        var lastText ='Last';
        var prevText ='« Previous';
        var nextText ='Next »';
        var urlactivepage=location.href;
        var home_page="/";

    if(typeof firstText=="undefined")firstText="First";if(typeof lastText=="undefined")lastText="Last";var noPage;var currentPage;var currentPageNo;var postLabel;pagecurrentg();function looppagecurrentg(pageInfo){var html='';pageNumber=parseInt(numPages / 2);if(pageNumber==numPages-pageNumber){numPages=pageNumber*2+1}
    pageStart=currentPageNo-pageNumber;if(pageStart<1)pageStart=1;lastPageNo=parseInt(pageInfo / perPage)+1;if(lastPageNo-1==pageInfo / perPage)lastPageNo=lastPageNo-1;pageEnd=pageStart+numPages-1;if(pageEnd>lastPageNo)pageEnd=lastPageNo;html+="<span class='showpageOf'>Page "+currentPageNo+' of '+lastPageNo+"</span>";var prevNumber=parseInt(currentPageNo)-1;if(currentPageNo>1){if(currentPage=="page"){html+='<span class="showpage firstpage"><a href="'+home_page+'">'+firstText+'</a></span>'}else{html+='<span class="displaypageNum firstpage"><a href="/search/label/'+postLabel+'?&max-results='+perPage+'">'+firstText+'</a></span>'}}
    if(currentPageNo>2){if(currentPageNo==3){if(currentPage=="page"){html+='<span class="showpage"><a href="'+home_page+'">'+prevText+'</a></span>'}else{html+='<span class="displaypageNum"><a href="/search/label/'+postLabel+'?&max-results='+perPage+'">'+prevText+'</a></span>'}}else{if(currentPage=="page"){html+='<span class="displaypageNum"><a href="#" onclick="redirectpage('+prevNumber+');return false">'+prevText+'</a></span>'}else{html+='<span class="displaypageNum"><a href="#" onclick="redirectlabel('+prevNumber+');return false">'+prevText+'</a></span>'}}}
    if(pageStart>1){if(currentPage=="page"){html+='<span class="displaypageNum"><a href="'+home_page+'">1</a></span>'}else{html+='<span class="displaypageNum"><a href="/search/label/'+postLabel+'?&max-results='+perPage+'">1</a></span>'}}
    if(pageStart>2){html+=' ... '}
    for(var jj=pageStart;jj<=pageEnd;jj++){if(currentPageNo==jj){html+='<span class="pagecurrent">'+jj+'</span>'}else if(jj==1){if(currentPage=="page"){html+='<span class="displaypageNum"><a href="'+home_page+'">1</a></span>'}else{html+='<span class="displaypageNum"><a href="/search/label/'+postLabel+'?&max-results='+perPage+'">1</a></span>'}}else{if(currentPage=="page"){html+='<span class="displaypageNum"><a href="#" onclick="redirectpage('+jj+');return false">'+jj+'</a></span>'}else{html+='<span class="displaypageNum"><a href="#" onclick="redirectlabel('+jj+');return false">'+jj+'</a></span>'}}}
    if(pageEnd<lastPageNo-1){html+='...'}
    if(pageEnd<lastPageNo){if(currentPage=="page"){html+='<span class="displaypageNum"><a href="#" onclick="redirectpage('+lastPageNo+');return false">'+lastPageNo+'</a></span>'}else{html+='<span class="displaypageNum"><a href="#" onclick="redirectlabel('+lastPageNo+');return false">'+lastPageNo+'</a></span>'}}
    var nextnumber=parseInt(currentPageNo)+1;if(currentPageNo<(lastPageNo-1)){if(currentPage=="page"){html+='<span class="displaypageNum"><a href="#" onclick="redirectpage('+nextnumber+');return false">'+nextText+'</a></span>'}else{html+='<span class="displaypageNum"><a href="#" onclick="redirectlabel('+nextnumber+');return false">'+nextText+'</a></span>'}}
    if(currentPageNo<lastPageNo){if(currentPage=="page"){html+='<span class="displaypageNum lastpage"><a href="#" onclick="redirectpage('+lastPageNo+');return false">'+lastText+'</a></span>'}else{html+='<span class="displaypageNum lastpage"><a href="#" onclick="redirectlabel('+lastPageNo+');return false">'+lastText+'</a></span>'}}
    var pageArea=document.getElementsByName("pageArea");var blogPager=document.getElementById("blog-pager");for(var p=0;p<pageArea.length;p++){pageArea[p].innerHTML=html}
    if(pageArea&&pageArea.length>0){html=''}
    if(blogPager){blogPager.innerHTML=html}}
    function totalcountdata(root){var feed=root.feed;var totaldata=parseInt(feed.openSearch$totalResults.$t,10);looppagecurrentg(totaldata)}
    function pagecurrentg(){var thisUrl=urlactivepage;if(thisUrl.indexOf("/search/label/")!=-1){if(thisUrl.indexOf("?updated-max")!=-1){postLabel=thisUrl.substring(thisUrl.indexOf("/search/label/")+14,thisUrl.indexOf("?updated-max"))}else{postLabel=thisUrl.substring(thisUrl.indexOf("/search/label/")+14,thisUrl.indexOf("?&max"))}}
    if(thisUrl.indexOf("?q=")==-1&&thisUrl.indexOf(".html")==-1){if(thisUrl.indexOf("/search/label/")==-1){currentPage="page";if(urlactivepage.indexOf("#PageNo=")!=-1){currentPageNo=urlactivepage.substring(urlactivepage.indexOf("#PageNo=")+8,urlactivepage.length)}else{currentPageNo=1}
    document.write("<script src=\""+home_page+"feeds/posts/summary?max-results=1&alt=json-in-script&callback=totalcountdata\"><\/script>")}else{currentPage="label";if(thisUrl.indexOf("&max-results=")==-1){perPage=20}
    if(urlactivepage.indexOf("#PageNo=")!=-1){currentPageNo=urlactivepage.substring(urlactivepage.indexOf("#PageNo=")+8,urlactivepage.length)}else{currentPageNo=1}
    document.write('<script src="'+home_page+'feeds/posts/summary/-/'+postLabel+'?alt=json-in-script&callback=totalcountdata&max-results=1" ><\/script>')}}}
    function redirectpage(numberpage){jsonstart=(numberpage-1)*perPage;noPage=numberpage;var nameBody=document.getElementsByTagName('head')[0];var newInclude=document.createElement('script');newInclude.type='text/javascript';newInclude.setAttribute("src",home_page+"feeds/posts/summary?start-index="+jsonstart+"&max-results=1&alt=json-in-script&callback=finddatepost");nameBody.appendChild(newInclude)}
    function redirectlabel(numberpage){jsonstart=(numberpage-1)*perPage;noPage=numberpage;var nameBody=document.getElementsByTagName('head')[0];var newInclude=document.createElement('script');newInclude.type='text/javascript';newInclude.setAttribute("src",home_page+"feeds/posts/summary/-/"+postLabel+"?start-index="+jsonstart+"&max-results=1&alt=json-in-script&callback=finddatepost");nameBody.appendChild(newInclude)}
    function finddatepost(root){post=root.feed.entry[0];var timestamp1=post.published.$t.substring(0,19)+post.published.$t.substring(23,29);var timestamp=encodeURIComponent(timestamp1);if(currentPage=="page"){var pAddress="/search?updated-max="+timestamp+"&max-results="+perPage+"#PageNo="+noPage}else{var pAddress="/search/label/"+postLabel+"?updated-max="+timestamp+"&max-results="+perPage+"#PageNo="+noPage}
    location.href=pAddress}

      /*]]>*/
    </script>
    <script type='text/javascript'>
      /*<![CDATA[*/
      (function(e,t,n,r){e.fn.sss=function(r){var i=e.extend({slideShow:true,startOn:0,speed:3500,transition:400,arrows:true},r);return this.each(function(){function y(e){return s.eq(e).height()/o.width()*100+"%"}function b(e){if(!c){c=true;var t=s.eq(e);t.fadeIn(a);s.not(t).fadeOut(a);o.animate({paddingBottom:y(e)},a,function(){c=false});g()}}function w(){l=l===u-1?0:l+1;b(l)}function E(){l=l===0?u-1:l-1;b(l)}var r=e(this),s=r.children().wrapAll('<div class="sss"/>').addClass("ssslide"),o=r.find(".sss"),u=s.length,a=i.transition,f=i.startOn,l=f>u-1?0:f,c=false,h,p,d,v,m,g=i.slideShow?function(){clearTimeout(p);p=setTimeout(w,i.speed)}:e.noop;if(i.arrows){o.append('<div class="sssprev"/>','<div class="sssnext"/>')}m=o.find(".sssnext"),v=o.find(".sssprev");e(t).load(function(){o.css({paddingBottom:y(l)}).click(function(t){h=e(t.target);if(h.is(m)){w()}else if(h.is(v)){E()}});b(l);e(n).keydown(function(e){d=e.keyCode;if(d===39){w()}else if(d===37){E()}})})})}})(jQuery,window,document)
      /*]]>*/
    </script>
    <script type='text/javascript'>
      /*<![CDATA[*/
            	// Get all Accordion and Panel
let accHeading = document.querySelectorAll(".accordion");
let accPanel = document.querySelectorAll(".panel");

for (let i = 0; i < accHeading.length; i++) {
    // Execute whenever an accordion is clicked
    accHeading[i].onclick = function() {
        if (this.nextElementSibling.style.maxHeight) {
           hidePanels();     // Hide All open Panels
        } else {
           showPanel(this);  // Show the panel
        }
    };
}

// Function to Show a Panel
function showPanel(elem) {
  hidePanels();
  elem.classList.add("active");
  elem.nextElementSibling.style.maxHeight = elem.nextElementSibling.scrollHeight + "px";
}

// Function to Hide all shown Panels
function hidePanels() {
  for (let i = 0; i < accPanel.length; i++) {
      accPanel[i].style.maxHeight = null;
      accHeading[i].classList.remove("active");
  }
}

            /*]]>*/
    </script>

    <!--/b:if>
    </b:if-->

  </body>
  <macro:includable id='sections' var='col'>
    <macro:if cond='data:col.num == 0'>
      <macro:else/>
      <b:section mexpr:class='data:col.class' mexpr:id='data:col.idPrefix + &quot;-1&quot;' preferred='yes' showaddelement='yes'/>
      <macro:if cond='data:col.num &gt;= 2'>
        <table border='0' cellpadding='0' cellspacing='0' mexpr:class='&quot;section-columns columns-&quot; + data:col.num'>
          <tbody>
            <tr>
              <td class='first columns-cell'>
                <b:section mexpr:class='data:col.class' mexpr:id='data:col.idPrefix + &quot;-2-1&quot;'/>
              </td>
              <td class='columns-cell'>
                <b:section mexpr:class='data:col.class' mexpr:id='data:col.idPrefix + &quot;-2-2&quot;'/>
              </td>
              <macro:if cond='data:col.num &gt;= 3'>
                <td class='columns-cell'>
                  <b:section mexpr:class='data:col.class' mexpr:id='data:col.idPrefix + &quot;-2-3&quot;'/>
                </td>
              </macro:if>
              <macro:if cond='data:col.num &gt;= 4'>
                <td class='columns-cell'>
                  <b:section mexpr:class='data:col.class' mexpr:id='data:col.idPrefix + &quot;-2-4&quot;'/>
                </td>
              </macro:if>
            </tr>
          </tbody>
        </table>
        <macro:if cond='data:col.includeBottom'>
          <b:section mexpr:class='data:col.class' mexpr:id='data:col.idPrefix + &quot;-3&quot;' showaddelement='no'/>
        </macro:if>
      </macro:if>
    </macro:if>
  </macro:includable>


<b:section-contents id='footer-1'>
  <b:widget cond='data:view.isHomepage' id='FeaturedPost1' locked='false' title='Entri yang Diunggulkan' type='FeaturedPost'>
    <b:widget-settings>
      <b:widget-setting name='showSnippet'>false</b:widget-setting>
      <b:widget-setting name='showPostTitle'>true</b:widget-setting>
      <b:widget-setting name='showFirstImage'>false</b:widget-setting>
      <b:widget-setting name='useMostRecentPost'>true</b:widget-setting>
    </b:widget-settings>
    <b:includable id='main'>
  <!-- Only display title if it's non-empty -->
  <b:if cond='data:title != &quot;&quot;'>
    <h2 class='title'><data:title/></h2>
  </b:if>
  <b:include name='content'/>

  <b:include name='quickedit'/>
</b:includable>
    <b:includable id='content'>
  <div class='post-summary'>
    <b:if cond='data:showPostTitle and data:postTitle != &quot;&quot;'>
      <h3><a expr:href='data:postUrl'><data:postTitle/></a></h3>
    </b:if>
    <b:if cond='data:showSnippet and data:postSummary != &quot;&quot;'>
      <p>
        <data:postSummary/>
      </p>
    </b:if>
    <b:if cond='data:showFirstImage and data:postFirstImage != &quot;&quot;'>
      <img class='image' expr:src='data:postFirstImage'/>
    </b:if>
  </div>

  <style type='text/css'>
    .image {
      width: 100%;
    }
  </style>
</b:includable>
  </b:widget>
</b:section-contents><b:section-contents id='footer-2-1'/><b:section-contents id='footer-2-2'/><b:section-contents id='footer-2-3'/></html>
