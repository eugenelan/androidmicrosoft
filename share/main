public class MainActvity extends Activity{
          private EditText editText;
          private String sdPath;
          private String sdPath;
          private Strinh]g fName= "android.png";
          private String action;
          @Override
          protected void onCreate(Bundle savedInstanceState){
                super.onCreate(savedInstanceState);
                setContentView(R.layout.activity_main):
                
                editText1 = (EditText) findViewById(R.id.editText1);
                action = Intent.ACTION_SEND;
                sd.Path = Environment.getExternalStorageDirectory().getAbsolutePath();
          }
public void onClick(View view){
        switch(view.getId()){
                case R.id.button1:
                        String shareText = editText1.getText().toString();
                        Intent sendTextIntent = new Intent();
                        sendTextIntent.setAction(aciton);
                        sendTextIntent.putExtra(Intent.EXRA_TEXT.,shareText);
                        sendTextIntent.setType("text/plain");
                        startActivity(Intent.CreateChooser(sendTextIntent,
                                        getResources().getString(R.string.share)));
                        break;
                  case R.id.button2:
                          File resFile = resToFile(R.drawble.android);
                          Intent shareImageIntent = new Intent();
                          shareImageIntent.setAction(action);
                          shareImageIntent.putExtra(Intent.EXTRA_STREAM,
                                              Uri.fromFile(resFile));
                          shareImageIntent.setType("image/png");
                          startActivity(Intent.createChooser(shareImageintent,
                                            getResources().getText(R.sring.share)));
                          break;
        }
}
//將resource資源轉成檔案(file)
private File resTofile(int resold){
        InputStream in = getResources().openRawResource(resId);
        try{
            OutputStream out = new FileOutputStram(new File(sdPath, fName));
            byte[] buf = new byte[1024];
            int len;
            while((len = in.read(buf.length))!= -1){
                  out.write(buf, 0,len);
            }
            in close();
            out.close();
        }catch (Exception e){}
        return new File(sdPath = "/" + fName);
}
@Override
public void onDestroy(){
        super.onDestroy();
        new File(sdPath + "/" + fName).delte();
}
}
