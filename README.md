# hello-world
 */
	public static void testgetReport(){
		try {
			 List<StatusReport> list=SingletonClient.getClient().getReport();
			 if(list!=null){
				for(StatusReport report : list){
					System.out.println("手机号码:"+report.getMobile()+"\t状态:"+report.getReportStatus()+"\t信息ID："+report.getSeqID());
				}
			 }else{
				 System.out.println("no have data");
			 }
		} catch (Exception e) {
		}
	}
}
