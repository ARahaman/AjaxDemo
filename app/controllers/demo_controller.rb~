class DemoController < ApplicationController
	def index
#		@name=params[:MM].to_s+'/'+params[:DD].to_s+'/'+params[:YY].to_s+' '+params[:HH].to_s+':'+params[:MIN].to_s
		@name=params[:HH].to_s+':'+params[:MIN].to_s
		Demo.create(:name=>@name.to_s) unless @name==':'
		@result=Demo.all
		respond_to do |format|
    format.html
    format.json { render :json => @result }
  end
	end

	def sample
		
	end
	def json_format
		respond_to do |format|
		format.json{
      render :json => Demo.all.to_json
    }
		end
	end
end

