<!DOCTYPE html>
<html>
    <head>
        <link rel="stylesheet" href="codebase/skins/touch.css" type="text/css" media="screen" charset="utf-8">
        <script src="codebase/webix.js" type="text/javascript" charset="utf-8"></script>
        <meta name="viewport" content="initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
        <title> Demo </title>
    </head>
    <body>
        <script>
            webix.ready(function() {
                var films = webix.ajax().sync().post("http://io.nowdb.net/collection/select_all.json",
                        {
                            "token": "533279628d909e0f0cfc42c6",
                            "project": "movie",
                            "collection": "films"
                        },
                function(text, xml, xhr) {
                    return text;
                });

                var datas = films.responseText;

                webix.ui.fullScreen();
                webix.ui({
                    rows: [
                        {view: "toolbar", elements: [
                                {view: "button", value: "Tambah", width: 100, type: "form", click: add_row},
                                {view: "button", value: "Ubah", width: 100, type: "form", click: update_row},
                                {view: "button", value: "Hapus", width: 100, type: "form", click:delete_row}
                            ]},
                        {cols: [
                                {view: "form", id: "myform", elements: [
                                        {view: "text", name: "title", placeholder: "Title", width: 500},
                                        {view: "text", name: "synopsis", placeholder: "Synopsis"},
                                        {view: "text", name: "rating", placeholder: "Rating"}

                                    ]},
                                {
                                    view: "list",
                                    id: "teks",
                                    height: 200,
                                    template: "#title#: #synopsis# dengan rating #rating#",
                                    select: true,
                                    data: datas
                                }
                            ]},
                        {
                            view: "multiview",
                            cells: [
                                {
                                    id: "title",
                                    view: "list",
                                    template: "#title#",
                                    data: datas,
                                    select: true
                                },
                                {
                                    id: "synopsis",
                                    view: "list",
                                    template: "#synopsis#",
                                    data: datas,
                                    select: true
                                },
                                {
                                    id: "rating",
                                    view: "list",
                                    template: "#rating#",
                                    data: datas,
                                    select: true
                                }

                            ]
                        },
                        {
                            view: "tabbar",
                            type: "iconTop",
                            multiview: true,
                            options: [
                                {id: "title", icon: "film", value: "Title"},
                                {id: "synopsis", icon: "user", value: "Sysnopsis"},
                                {id: "rating", icon: "tags", value: "Rating"}
                            ]

                        }
                    ]
                }

                );
                function add_row() {
                    var values = {
                        "token": "533279628d909e0f0cfc42c6",
                        "project": "movie",
                        "collection": "films",
                        title: $$("myform").getValues().title,
                        synopsis: $$("myform").getValues().synopsis,
                        rating: $$("myform").getValues().rating};
                    webix.ajax().post("http://io.nowdb.net/collection/insert", values, function() {
                        webix.message({type: "debug", text: "Films is save", expire: -1});
                    });
                }
                function update_row() {
                    var values = {
                        "token": "533279628d909e0f0cfc42c6",
                        "project": "movie",
                        "collection": "films"
                       
                    };
                    var sel = $$("teks").getSelectedId(); //checks whether the item is selected
    if(!sel) return;
                    var value1 = $$('myform').getValues().title;
                    var value2 = $$('myform').getValues().synopsis;
                    var value3 = $$('myform').getValues().rating;

                    for (var i = 0; i < sel.length; i++) {
                        var item = $$("teks").getItem(sel[i]); //for every selected item
                        item.title = value1; //setting values for list item
                        item.synopsis = value2;
                        item.rating = value3;
                        $$("teks").updateItem(sel[i], item); //updating
                    }
                    webix.ajax().post("http://io.nowdb.net/collection/update_id", values, function() {
                        webix.message({type: "debug", text: "Films is update", expire: -1});
                    });
                 }
                function delete_row() {
                    var values={
                        "token": "533279628d909e0f0cfc42c6",
                        "project": "movie",
                        "collection": "films",
                        id: $$("teks").getSelectedId()
                    };
                     webix.ajax().post("http://io.nowdb.net/collection/delete_id", values, function() {
                        webix.message({type: "debug", text: "Films is delete", expire: -1});
                    });
                    
                }
            });
        </script>
    </body>
</html>
