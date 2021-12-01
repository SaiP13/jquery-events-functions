# jquery-events-functions
All jQuery Functions and Events
<hr>

SELECTORS:

    1) #using class name   :     $('.class_name')
    2) #using ID name      :     $('#id_name')
    3) #uing tag name      :     $('tagname')
    4) #using ele & class  :     $("p.class_name")
    5) #all elements       :     $("a[href]") || $("a[target='_blank']") || $(":button")

GETTING VALUES:

    1) var x = $("#id_name").val();
    2) var x = $(".class_name").val();
    3) var x = $(this).val();
    4) var x = $(this).attr('attribute-name');
    5) var str = $("form").serialize(); || $(this).serialize();
    6) var checked_val = $("input:checkbox[name=check_coll]:checked").val(); #checkbox value
    7) var radio_val = $("input:radio[name=status]:checked").val(); #radio value
    8) var x = $("input:checkbox").val();
    9) $('#id').each(function(){ var x = $(this).val(); });
    10) $('.class').each(function(){ var x = $(this).val(); });

EVENTS:

    #MOUSE EVENTS:
        
        <!-- Click Statrt -->
        1) $("#id").click(function(){ }); #using id name
        2) $(".class_name").click(function(){ }); #using class name
        3) $(document).on("click", ".edit_listcontact", function(){ }); #using class name
        4) $(document).on("click","#upd_user_info_btn",function(){ });  #using id name
        <!-- Click End -->

        <!-- Double Click -->
        1) $("p").dblclick(function(){ });
        2) $("#id").dblclick(function(){ });
        3) $(".class").dblclick(function(){ }); 
        <!-- Double Click End -->

        <!--  Mouse Enter -->
        1) $("p").mouseenter(function(){ });
        2) $("#id").mouseenter(function(){ });
        3) $(".class").mouseenter(function(){ }); 
        <!--  End Mouse Enter -->

        <!--  Mouse leave -->
        1) $("p").mouseleave(function(){ });
        2) $("#id").mouseleave(function(){ });
        3) $(".class").mouseleave(function(){ }); 
        <!--  End Mouse Leave -->

        <!--  Mouse Down -->
        1) $("p").mousedown(function(){ });
        2) $("#id").mousedown(function(){ });
        3) $(".class").mousedown(function(){ }); 
        <!--  End Mouse Down -->

        <!--  Mouse leave -->
        1) $("p").mouseup(function(){ });
        2) $("#id").mouseup(function(){ });
        3) $(".class").mouseup(function(){ }); 
        <!--  End Mouse Leave -->

        <!-- Hover -->
        1) $("p").hover(function(){ });
        2) $("#id").hover(function(){ });
        3) $(".class").hover(function(){ }); 
        <!--  End Hover -->

    #FORM EVENTS:
    
        <!-- Form submit -->
        1) $("form").submit(function(){ });
        2) $("#form_id").submit(function(){ });
        3) $(".form_class").submit(function(){ }); 
        <!-- End Submit -->

        <!-- Change -->
        # when an input field is changed || value enter and remove
        1) $("input").change(function(){ });
        2) $("#input_id").change(function(){ });
        3) $(".input_class").change(function(){ }); 
        <!-- End Change -->

        <!--  Focus -->
        #when the form field gets focus || enter into form input filed

        1) $("input").focus(function(){ });
        2) $("#id").focus(function(){ });
        3) $(".class").focus(function(){ }); 
        <!--  End Focus -->

        <!--  Blur -->
        #when the form field lose focus || leave form input filed

        1) $("input").blur(function(){ });
        2) $("#id").blur(function(){ });
        3) $(".class").blur(function(){ }); 
        <!--  End Blur -->
    
    #KEYBOARD EVENTS:

        <!-- Key Down -->
        # when <input> field when a keyboard key is pressed down.

        1) $("input").keydown(function(){ });
        2) $("#input_id").keydown(function(){ });
        3) $(".input_class").keydown(function(){ }); 
        <!-- End Key Down -->

        <!-- Key Up -->
        # when an <input> field when a keyboard key is released.

        1) $("input").keyup(function(){ });
        2) $("#input_id").keyup(function(){ });
        3) $(".input_class").keyup(function(){ }); 
        <!-- End Key Up -->

        <!-- Key Press -->
        # when <input> field when a keyboard key is pressed.

        1) $("input").keypress(function(){ });
        2) $("#input_id").keypress(function(){ });
        3) $(".input_class").keypress(function(){ }); 
        <!-- End Key Press -->

    #MULTIPLE EVENTS AT A TIME:
    
        <!-- on -->
        1) $("input").on('click','blur', function(){ });
        2) $("#input_id").on('keypress','hover', function(){ });
        3) $(".input_class").on('keypress','hover',function(){ });
        4) $('#account_id').on('change', function () { });
        5) $(document).on("keyup","#id-name",function(){});
        5) $(document).on("keyup",".class-name",function(){});
        7) $("selector").on({  
                        mouseenter: function(){ $(this).css("background-color", "lightgray"); },
                        mouseleave: function(){ $(this).css("background-color", "lightblue"); }, 
                        click: function(){ $(this).css("background-color", "yellow"); }
                    });
        <!-- end on -->


$(document).on("click", ".edit_listcontact", function(){ });

$(document).on("click","#upd_user_info_btn",function(){ });

$(document).on("keyup","#statesearch",function(e){});

$('#account_id').on('change', function () { });

$('#ultab a[href="#add_contacts"]').click(function(){ });

$("#contact_per_salutation").addClass("errTxtField");

$("#contact_per_salutation").removeClass("errTxtField");

$(document).one('click', closeTooltip);

$(".loader").show();

$("#show_parent_grp").hide(); 

$(".loader").append();

$('#reporting_to_contact_person').empty();

$('#imagepopup').modal('show');

$('#image-zoom').attr("src",img_path);

$('#users_for_account').append($("<option></option>").attr("value",0).text("Select"));

$('input').on('ifChecked', function(event){ });

$('input').on('ifUnchecked', function(event){ });

$.each(response.products, function(key,value) { });

if(!mailValidation(assistant_email)){}

$("#closepop" ).trigger( "click" );

$(".modal-title").html("Edit Notification");

$("#all_regn_chkd").prop("checked",true);

$('#gst_chk_1').prop('checked', false);

$('input:checkbox.stateBoxClass').each(function () { });

$(".sta_cls").css("display","block");

$(".sta_cls").css("display","none");

$("input[type=radio][name=team_for]:checked").val();

$("#member_designation").keypress(function () { });

$("input[name='gst_chk']").serializeArray();

$("#pan,#company,#address").val('');

var formData = new FormData($("#form-usermanagement")[0]);
