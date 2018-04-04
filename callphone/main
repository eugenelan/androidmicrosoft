public class MainActivity extends Activity{
          private EditText editText;
          private Context caontext;
          private String action;
          @Override
          public void onCreate(Bundle savedInstanceState){
                  super.onCreate(savedInstanceState);
                  setContentView(R.layout.activity_main);
                  context = this;
                  action = Intent.ACTION_CALL;
                  editText = (EditText)this.findViewById(R.id.editText);
          }
          
          public void onClick(View view){
                   switch(view.getId()){
                          case R.id.button1:
                                   String phoneNumber = editText1.getText().toString();
                                   if((phoneNumber == null) || (phoneNumber.equals(""))){
                                          Toast.makeTExt(context, R.string.message,
                                                          Toast.LENGTH_SHORT).show();
                                   }else{
                                          Uri uri = Uri.parse("tel:"+ phoneNumber);
                                          Intent intent = new Intent(action,uri);
                                          startActivity(intent);
                                   }break;
                   }
          }
}
